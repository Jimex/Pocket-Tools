# Music Tango

Music Tango is an Android music player for local MP3/FLAC libraries, internet radio, and music downloads. It shows synchronized lyrics for songs and can transcribe radio speech into live subtitles on the device with Whisper.

- **Package:** `cn.jimex.musictango`
- **Version:** 1.0.1.2 (versionCode 1012) · [Release notes](docs/RELEASE_NOTES.md)
- **Min SDK:** 26 (Android 8.0) · **Target SDK:** 36 · **Compile SDK:** 37
- **Languages:** English, Simplified Chinese, Traditional Chinese

For end-user instructions, see the User Manual: [English](docs/USER_MANUAL.md) · [简体中文](docs/USER_MANUAL.zh-CN.md) · [繁體中文](docs/USER_MANUAL.zh-TW.md). The build also packages `docs/` as APK assets, and the app shows the manuals under **Settings → About → User manual**, so any edit to them ships with the next build.

## Features

| Area | What it does |
|------|--------------|
| Library | Scans the device or a SAF-selected folder for audio and adds the tracks you pick to the library. You can search, sort, edit metadata, give tracks a category, and filter by category or **Recently added**. |
| Music file tags | Metadata edits and saved lyrics are written back into the MP3 (ID3v2.3/2.4) or FLAC (Vorbis comment) file, and read back on import, so they survive a reinstall. Can be turned off in Settings. |
| Playback | Media3 ExoPlayer in a `MediaSessionService`, with background playback, notification and lock-screen controls, a reorderable play queue, and repeat-all / repeat-one / shuffle modes. |
| Now Playing | Songs: vinyl-style player with selectable tonearm styles and custom cover art (from the device, an image URL, or Google Images search). Radio: an Audio wave or Classic radio visual driven by the real audio levels, previous/next station controls, and a live transcription toggle. |
| Lyrics | LRC lyrics fetched from an LrcApi-compatible service (default `https://api.lrc.cx/lyrics`), cached in Room. You can also import a `.lrc` file, generate lyrics on the device with Whisper or Fun-ASR, and edit them in a full-screen editor with tap-to-sync, a waveform timeline, validation and AI re-timing. The current line is highlighted, and tapping a line seeks to it. |
| Playlists | Create, rename, delete and reorder playlists, and import or export them. |
| Radio | Saved internet radio stations. You can add a stream URL by hand or search the [Radio Browser](https://www.radio-browser.info/) directory. |
| Radio transcription | On-device Whisper (whisper.cpp through JNI) transcribes radio speech into live subtitles, with an adjustable subtitle delay. Transcription is turned on per station, from the Radio tab or from Now Playing. |
| Downloader | **API Downloader:** search several music sources, pick a bitrate and preview a result before downloading. **Browser Downloader:** an embedded WebView. Both offer rename-before-save, a category and playlist for the download, duplicate handling, a download queue and history, and saving to a SAF folder. |
| Settings | Theme (system/light/dark, Material 3 dynamic color), language, data backup and restore, music file tag write-back, lyrics storage, font size and the Fun-ASR model, cover cache folder, radio visual, Whisper model management, and an About section with the version and the in-app user manual. |

## Permissions

| Permission | Purpose |
|------------|---------|
| `READ_MEDIA_AUDIO` (API 33+) / `READ_EXTERNAL_STORAGE` (≤ API 32) | Scan local music |
| `INTERNET` | Streaming, radio, lyrics, downloads, model downloads |
| `FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_MEDIA_PLAYBACK` | Background playback |
| `POST_NOTIFICATIONS` | Playback notification |
| `WRITE_EXTERNAL_STORAGE` (≤ API 28) | Write edited tags and lyrics into music files. On API 29+ the app asks for MediaStore write approval per file instead. |

The manifest enables cleartext HTTP traffic because many radio streams still use `http://`.

## Third-party services

The app talks to these external services. Their availability and terms are outside the project's control:

- LrcApi-compatible lyrics/cover service (`api.lrc.cx` by default; configurable)
- Radio Browser API (`*.api.radio-browser.info`)
- GD Studio music API (`music-api.gdstudio.xyz`) for the API Downloader
- Hugging Face `ggerganov/whisper.cpp` for Whisper model downloads
- Hugging Face `litert-community/Fun-ASR-Nano-2512` for the Fun-ASR lyrics model (run with LiteRT-LM)

Users are responsible for downloading only content they have the right to use.

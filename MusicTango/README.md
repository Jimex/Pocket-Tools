# Music Tango

Music Tango is an Android music player for local MP3/FLAC libraries, internet radio, and music downloads. It shows synchronized lyrics for songs and can transcribe radio speech into live subtitles on the device with Whisper.

- **Package:** `cn.jimex.musictango`
- **Version:** 1.0.1.1 (versionCode 1011)
- **Min SDK:** 26 (Android 8.0) · **Target SDK:** 36 · **Compile SDK:** 37
- **Languages:** English, Simplified Chinese, Traditional Chinese

For end-user instructions, see the User Manual: [English](docs/USER_MANUAL.md) · [简体中文](docs/USER_MANUAL.zh-CN.md) · [繁體中文](docs/USER_MANUAL.zh-TW.md).

## Features

| Area | What it does |
|------|--------------|
| Library | Scans the device or a SAF-selected folder for audio and adds the tracks you pick to the library. You can search, sort and edit metadata. |
| Playback | Media3 ExoPlayer in a `MediaSessionService`, with background playback, notification and lock-screen controls, a reorderable play queue, and repeat-all / repeat-one / shuffle modes. |
| Now Playing | Vinyl-style player with selectable tonearm styles and custom cover art (from the device, an image URL, or Google Images search). |
| Lyrics | LRC lyrics fetched from an LrcApi-compatible service (default `https://api.lrc.cx/lyrics`), cached in Room. You can also import a `.lrc` file or paste lyrics. The current line is highlighted, and tapping a line seeks to it. |
| Playlists | Create, rename, delete and reorder playlists, and import or export them. |
| Radio | Saved internet radio stations. You can add a stream URL by hand or search the [Radio Browser](https://www.radio-browser.info/) directory. |
| Radio transcription | On-device Whisper (whisper.cpp through JNI) transcribes radio speech into live subtitles, with an adjustable subtitle delay. Transcription is turned on per station. |
| Downloader | **API Downloader:** search several music sources and pick a bitrate. **Browser Downloader:** an embedded WebView. Both offer rename-before-save, duplicate handling, a download queue and history, and saving to a SAF folder. |
| Settings | Theme (system/light/dark, Material 3 dynamic color), language, lyrics storage and font size, cover cache folder, Whisper model management, and full data backup and restore. |


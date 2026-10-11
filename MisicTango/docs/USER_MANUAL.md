# Music Tango User Manual

Version 1.0.1.1 · English · [简体中文](USER_MANUAL.zh-CN.md) · [繁體中文](USER_MANUAL.zh-TW.md)

Music Tango plays your local music, streams internet radio, shows synchronized lyrics, and downloads music. It can also turn radio speech into live subtitles. The transcription runs entirely on your phone.

---

## Contents

1. [Getting started](#1-getting-started)
2. [Finding your way around](#2-finding-your-way-around)
3. [Building your library](#3-building-your-library)
4. [Playing music](#4-playing-music)
5. [The Now Playing screen](#5-the-now-playing-screen)
6. [Lyrics](#6-lyrics)
7. [Playlists](#7-playlists)
8. [Radio](#8-radio)
9. [Live radio transcription](#9-live-radio-transcription)
10. [Downloading music](#10-downloading-music)
11. [Settings](#11-settings)
12. [Backing up your data](#12-backing-up-your-data)
13. [Troubleshooting](#13-troubleshooting)

---

## 1. Getting started

**Requirements:** Android 8.0 or later. Live transcription needs a reasonably recent phone and a few hundred MB of free space for a speech model.

The first time you open Music Tango:

1. **Allow access to music/audio** when Android asks. The app needs it to find songs on your device.
2. **Allow notifications** so playback controls appear in the notification shade and on the lock screen.
3. Your library starts out empty. To fill it, follow [Building your library](#3-building-your-library).

---

## 2. Finding your way around

The navigation bar at the bottom of the screen has five tabs:

| Tab | What's there |
|-----|--------------|
| **Home** | Your song library, search, and the Scan music option |
| **Playlists** | Your playlists |
| **Radio** | Saved radio stations |
| **Browser** | The music downloader |
| **Settings** | App preferences |

When something is playing, a **mini player** appears above the navigation bar:

- Tap it to open the full **Now Playing** screen.
- Use its play/pause button to pause or resume without leaving the current screen.
- Open the **queue** from the mini player to see what will play next.

---

## 3. Building your library

### Scanning for music

1. On **Home**, open the menu and choose **Scan music**. If the library is empty, the button is shown on the screen.
2. Choose where to look:
   - **Scan device** searches all audio files Android knows about.
   - **Choose folder** lets you pick a folder, for example on an SD card. Only that folder is scanned.
3. The results show how many files were found. Songs that are already in your library are marked **In Library**.
4. Use **Sort** to order the results by **Name**, **Artist Name** or **Last Modified**, either ascending or descending. The search box filters the list by name or artist.
5. Tick the songs you want, or use **Select all**, then tap **Add selected**.

### Searching and managing songs

- The search on **Home** matches title, artist, album and file path.
- Tap a song to play it.
- Tap a song's **More** (⋮) button to:
  - **Add to queue** after the current song
  - **Add to playlist**
  - **Edit metadata** to change the title, artist or album shown in the app
  - **Remove from library**. This removes the song from Music Tango only. The audio file stays on your device.

---

## 4. Playing music

Playback continues in the background. You can control it from the notification, the lock screen, Bluetooth headsets and car systems.

### Playback modes

Tap the **playback mode** button to cycle through three modes:

| Mode | Behavior |
|------|----------|
| **Repeat all** | Plays the queue in order and starts again from the top (default) |
| **Repeat one** | Repeats the current song |
| **Shuffle** | Plays the queue in random order |

### The play queue

Open the queue from the mini player or the Now Playing screen. In the queue you can:

- Tap a song to jump to it.
- **Long-press and drag** a song to reorder it.
- Tap **✕** to remove a song from the queue.
- Use **Clear queue** to empty it.

---

## 5. The Now Playing screen

Now Playing shows the song on a spinning vinyl record, with the seek bar, previous/next, play/pause and the playback mode button.

- **Change the tonearm:** tap the tonearm's pivot to choose a style: Default, Black, Golden, Modern, Old Days, Steampunk or Cyberpunk.
- **Change the cover art:** tap the cover to open the cover art menu, then:
  - **Pick picture from device**
  - **Use image URL** to paste a link to an image
  - **Search Google Images** to search the web and **Use as cover**
  - **Clear cache for this song** to go back to the automatic cover
- **Lyrics:** the current lyric line appears below the record. Tap it to open the full lyrics view.

---

## 6. Lyrics

When a song starts, Music Tango looks up synchronized (LRC) lyrics using the title, artist and album. Lyrics it finds are saved, so they also work offline later.

In the lyrics view:

- The current line is highlighted, and the view scrolls with the music.
- Tap a line's **▶** to **play from here**, which jumps the song to that line.
- Use **A− / A+** to make the text smaller or larger.
- If no lyrics were found, or they are wrong:
  - **Import LRC** loads a `.lrc` file from your device.
  - **Paste or enter lyrics** lets you type or paste lyrics in, either plain or LRC format with `[mm:ss.xx]` timestamps.

You can change the lyrics storage folder and default font size in [Settings → Lyrics](#lyrics).

---

## 7. Playlists

Open the **Playlists** tab.

- **Create a playlist:** tap **+** and enter a name.
- **Open a playlist:** tap it. From there you can:
  - **Play this list** from the top, or tap a song to start from that song
  - **Add songs:** search your library, tick songs, then tap **Add**
  - **Remove** songs
  - **Move up / Move down** to reorder songs
- **Rename** or **Delete** a playlist from its menu. Deleting a playlist doesn't delete any songs.
- **Export / Import** a playlist to share it or move it to another device.

---

## 8. Radio

Open the **Radio** tab to see your saved stations. Tap a station to start listening. Live streams show a **LIVE** badge, and you can't seek within them.

### Adding stations

- **Search radio stations:** search the free Radio Browser directory by name, then tap **Add** next to a result.
- **Add Custom Station:** enter a **Station Name** and a **Stream URL** (for example an `.mp3`, `.aac` or `.m3u8` stream link).

To remove a station, use **Delete station** from its menu.

---

## 9. Live radio transcription

Music Tango can show live subtitles for spoken radio, such as news, talk shows and podcasts. It uses the Whisper speech-recognition model, which runs on your phone. No audio is uploaded.

### Step 1: Get a model

1. Go to **Settings → Transcription → Download models**.
2. Pick a model and tap **Download**. Then tap **Use** to make it active.

| Model | Size | Notes |
|-------|------|-------|
| Tiny | ~75 MB | Fastest. Good for older phones. |
| Base | ~142 MB | Better accuracy |
| Small (quantized) | ~183 MB | Close to Small accuracy at a smaller size |
| Small | larger | Best accuracy, slowest |

- **English** models only understand English and are a little more accurate for it.
- **Multilingual** models detect the spoken language automatically.

If you already have a GGML/GGUF Whisper model file, you can use **Choose file** under **Whisper model file** instead. Use **Test model** to check that it loads.

### Step 2: Turn transcription on for a station

On the **Radio** tab, open a station's menu and choose **Enable transcription**. Stations with transcription turned on are highlighted.

### Step 3: Listen

Play the station and open **Now Playing** or the lyrics view. Subtitles appear as the speech is recognized. The status line shows what the app is doing:

- *Connecting to radio stream* / *Decoding radio audio*
- *Transcribing N s of audio*
- *Listening – no speech detected yet* (normal during music)

**Tips**

- Expect the first subtitle to take several seconds.
- If the subtitles run ahead of or behind the audio, adjust **Settings → Transcription → Radio subtitle delay**.
- Transcription stops while the screen is off. Turn the screen on to resume subtitles.
- Transcription uses a lot of processing power and battery. Smaller models use less.

---

## 10. Downloading music

Open the **Browser** tab. It has two downloaders.

### API Downloader

1. Type a song name in **Search songs…**.
2. Open **Search settings** to choose:
   - **Source**: NetEase, QQ Music, Kuwo, Tidal, Qobuz, JOOX, Bilibili, Apple Music, YouTube Music or Spotify
   - **Bitrate**: from 128K Standard (under 3 MB per song) up to 24-bit Lossless (over 50 MB per song)
3. Tap **Download** on a result. A result marked *link unavailable* can't be downloaded from that source, so try another source.

### Browser Downloader

A built-in web browser. Type a web address or search term in **Search or type URL** and browse to a page with an audio file. When you start a download, the app asks where to save it. **Address history** brings back pages you visited earlier.

### The Save as dialog

Before a file is saved, you can:

- Edit the **File name**. The app won't accept characters that aren't allowed in file names.
- Choose to **Save under artist folder**.
- Choose the **Save location**: the default **Music** folder or a folder you picked.

If a file with the same name already exists, choose **Overwrite** or **Rename**.

Downloaded songs are added to your library automatically.

### Queue, history and folder

From **Browser Actions** (⋮):

- **Download Queue** shows downloads in progress.
- **Download History** lists past downloads and whether each one succeeded or failed.
- **Download folder** changes where files are saved. You can pick an SD card folder, and the app keeps access to it after restarts.

> Only download music you have the right to download.

---

## 11. Settings

### Theme
**System**, **Light** or **Dark**. On Android 12 and later, colors follow your wallpaper.

### Language
**System**, **English**, **Simplified Chinese** or **Traditional Chinese**.

### Lyrics
- **Lyrics storage folder:** where lyric files are kept. **Use default** keeps them inside the app.
- **Default lyrics font size**
- **Clear Cache** deletes saved lyrics so they are downloaded again.

### Cover art
- **Cover cache folder:** where downloaded cover images are kept. The default app folder is deleted when you uninstall the app. Choose another folder if you want to keep the covers.

### Transcription
- **Whisper model file / Download models:** see [Live radio transcription](#9-live-radio-transcription).
- **Radio subtitle delay** shifts subtitles so they line up with the audio.

---

## 12. Backing up your data

Go to **Settings → Data backup**.

- **Export data** saves your library, playlists, lyrics cache, download history and radio stations to a file you choose.
- **Import data** restores from a backup file.

> **Warning:** Importing a backup *replaces* all current app data on the device.

Backups contain the app's records, not the audio files themselves. If you restore on a different phone, the songs must also be on that phone.

---

## 13. Troubleshooting

| Problem | What to try |
|---------|-------------|
| No songs found when scanning | Check that Music Tango has the music/audio permission in Android Settings → Apps. Try **Choose folder** and pick the folder directly. |
| Wrong or missing lyrics | Use **Import LRC** or **Paste or enter lyrics**. Check that the song's title and artist are correct with **Edit metadata**. |
| Radio station won't play | The stream may be offline or the URL may have changed. Search for the station again in **Search radio stations**. |
| "Select a Whisper model file in Settings…" | Download and **Use** a model under **Settings → Transcription → Download models**. |
| "Unable to load Whisper model" | The file may be incomplete or not a Whisper GGML/GGUF model. Delete it and download it again, or try a smaller model. |
| "Offline transcription is unavailable…" | Your device may not support the model. Try a smaller model, such as **Tiny**. |
| Subtitles stop with the screen off | This is expected. Turn the screen on to resume. |
| Subtitles out of sync | Adjust **Radio subtitle delay** in Settings. |
| Download fails | Try a different **Source** or a lower **Bitrate**. Check that the download folder is still accessible, and choose it again if needed. |
| Playback controls missing from the notification | Allow notifications for Music Tango in Android Settings. |

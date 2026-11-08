# Music Tango User Manual

Version 1.0.1.2 · English · [简体中文](USER_MANUAL.zh-CN.md) · [繁體中文](USER_MANUAL.zh-TW.md)

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
- The chips above the song list filter it. **Recently added** shows your newest songs first, with the date each one was added. Once songs have a category, tap **All** or a category to show only that category. The filters work together with search.
- Tap a song to play it.
- Tap a song's **More** (⋮) button to:
  - **Add to queue** after the current song
  - **Add to playlist**
  - **Edit metadata** to change the title, artist, album or category
  - **Remove from library**. This removes the song from Music Tango only. The audio file stays on your device.

### Edits are saved into the music file

For MP3 and FLAC files, Music Tango also writes your metadata edits, including the category, and any lyrics you save into the music file itself. If you reinstall the app or clear the library, scanning the songs again brings the edits and lyrics back.

- When the app needs to change a file, Android may ask you to allow it. If you decline, or the file can't be changed safely, the edit is kept in Music Tango only and a message tells you so.
- To keep edits in the app only, turn off **Settings → Music files → Save edits into music files**.

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

### Songs

Now Playing shows the song on a spinning vinyl record, with the seek bar, previous/next, play/pause and the playback mode button.

- **Change the tonearm:** tap the tonearm's pivot to choose a style: Default, Black, Golden, Modern, Old Days, Steampunk or Cyberpunk.
- **Change the cover art:** tap the cover to open the cover art menu, then:
  - **Pick picture from device**
  - **Use image URL** to paste a link to an image
  - **Search Google Images** to search the web and **Use as cover**
  - **Clear cache for this song** to go back to the automatic cover
- **Lyrics:** the current lyric lines appear below the record. Tap them, or swipe left, to open the full lyrics page.

### Radio

For a radio station, Now Playing shows a radio visual instead of the record.

- **Change the visual:** tap the palette button at the top to switch between **Audio wave** and **Classic radio**. You can also choose it in [Settings → Radio](#radio-1).
- The visual moves with the sound that is playing. If you'd rather save a little battery, turn off **Follow the real audio** in Settings and it plays a decorative animation instead.
- The **LIVE Stream** bar replaces the seek bar, because you can't seek in a live stream. The subtitles button at its end turns [live transcription](#9-live-radio-transcription) on or off for this station.
- **Previous station** and **Next station** step through your saved stations, and wrap around at the end of the list.
- The live subtitles appear below the visual. Swipe left to see the full transcript.

---

## 6. Lyrics

When a song starts, Music Tango looks up synchronized (LRC) lyrics using the title, artist and album. Lyrics it finds are saved, so they also work offline later.

### The lyrics page

On Now Playing, swipe left or tap the lyric lines to open the lyrics page.

- The current line is highlighted, and the page scrolls with the music.
- Tap a line's **▶** to **play from here**, which jumps the song to that line.
- The **Lyrics options** (⋮) menu has:
  - **Generate lyrics with AI…**: see [below](#generating-lyrics-with-ai)
  - **Import LRC file…** loads a `.lrc` file from your device
  - **Enter lyrics…** or **Edit lyrics…** opens the [lyrics editor](#editing-lyrics)
  - **Text size…** makes the text smaller or larger
- When a song has no lyrics, the page offers the same choices directly.

### Generating lyrics with AI

Music Tango can listen to the song and write the lyrics for you. It runs on your phone.

1. Choose **Generate lyrics with AI…**.
2. Pick a **Model** and the song's language, or **Auto-detect**. The app remembers your choice for next time.
3. Tap **Generate**. Progress is shown above the lyrics, and you can cancel. A long song can take a few minutes.

The first line of generated lyrics notes which model made them. If the song already had lyrics, the old lyrics file is moved to an `archive` folder.

You can choose from two kinds of model:

| Model | Get it from | Good for |
|-------|-------------|----------|
| **Whisper** | Settings → Transcription → **Download models** (the same models as live radio transcription) | Many languages. Gives line times. |
| **Fun-ASR** | Settings → Lyrics → **Lyrics generation models** | Much better at sung lyrics and Chinese dialects such as Cantonese. Chinese, English and Japanese only. About 1.26 GB, plus about 1.5 GB prepared on first use. Needs a 64-bit phone. Line times are estimated. |

Sung vocals are harder to recognize than speech, so check the result and fix it in the editor.

### Editing lyrics

The lyrics editor fills the screen and has two tabs:

- **Lines** lists every line with its time. Tap a line to select it, then edit its text or use **−0.1s** / **+0.1s** to fine-tune its time. Each line also has buttons to **Play from this line**, **Insert line below** and **Delete line**. Use **Add line** to add one at the end.
- **LRC text** shows the lyrics as plain text. Paste LRC lyrics with `[mm:ss.xx]` times, or plain lyrics without times.

**Syncing lines to the music.** Play the song, select a line and tap **Sync line** as that line starts. The next line is selected for you, so you can tap through the whole song. **Back 3 seconds** and **Forward 3 seconds** help you catch a line again. The timing tools work only while this song is the one playing.

**More editing options** (⋮):

- **Shift lines…** moves the **Selected line**, the **Selected line and all after it**, or **All lines** earlier or later by the number of seconds you enter.
- **Sort lines by time**
- **Re-time with AI…** listens to the song and moves the times of the lines it can match, including lines with no time yet. Your text isn't changed.
- **Show waveform** adds a timeline of the song's loudness with a marker for each line. Tap a marker to select its line, drag the selected marker to change its time, or tap elsewhere to jump there.

**Review** lists possible problems: lines with no time, unreadable times, lines out of order, duplicate lines, very long lines and times past the end of the song. Tap a problem to jump to its line.

**Undo** and **Redo** are at the top. Tap **Save** when you're done. If some lines still have no time, the app asks before saving, because those lines won't show during playback. If you leave without saving, the app asks whether to discard your changes.

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

Either:

- On the **Radio** tab, open a station's menu and choose **Enable transcription**. Stations with transcription turned on are highlighted.
- While the station plays, tap the subtitles button at the end of the **LIVE Stream** bar on Now Playing. When transcription is off, you can also tap the subtitle area under the radio visual, or **Turn on live transcription** on the transcript page.

The station restarts briefly to switch over. Tap the subtitles button again to turn transcription off.

### Step 3: Listen

Play the station and open **Now Playing**. Subtitles appear under the radio visual as the speech is recognized. Swipe left for the full transcript. The status line shows what the app is doing:

- *Connecting to radio stream* / *Decoding radio audio*
- *Transcribing N s of audio*
- *Listening – no speech detected yet* (normal during music)

**Tips**

- Expect the first subtitle to take several seconds.
- If the subtitles run ahead of or behind the audio, adjust **Settings → Transcription → Radio subtitle delay**.
- Transcription stops while the screen is off. Turn the screen on to resume subtitles.
- Transcription uses a lot of processing power and battery. Smaller models use less.
- Transcribed radio pauses when another app plays sound, during a phone call, or when you unplug your headphones, just like regular playback.

---

## 10. Downloading music

Open the **Browser** tab. It has two downloaders.

### API Downloader

1. Type a song name in **Search songs…**.
2. Open **Search settings** to choose:
   - **Source**: NetEase, QQ Music, Kuwo, Tidal, Qobuz, JOOX, Bilibili, Apple Music, YouTube Music or Spotify
   - **Bitrate**: from 128K Standard (under 3 MB per song) up to 24-bit Lossless (over 50 MB per song)
3. Tap **Preview** (the play button) on a result to listen before downloading. Tap it again to pause, and drag the bar under the result to skip ahead. Starting a preview pauses whatever the player was playing.
4. Tap **Download** on a result. A result marked *link unavailable* can't be downloaded from that source, so try another source.

### Browser Downloader

A built-in web browser. Type a web address or search term in **Search or type URL** and browse to a page with an audio file. When you start a download, the app asks where to save it. **Address history** brings back pages you visited earlier.

### The Save as dialog

Before a file is saved, you can:

- Edit the **File name**. The app won't accept characters that aren't allowed in file names.
- Choose to **Save under artist folder**.
- Choose the **Save location**: the default **Music** folder or a folder you picked.
- Type a **Category**, or pick one you've used before from the list.
- Pick a playlist under **Add to playlist** to add the song there once it's downloaded.

The dialog remembers the last category and playlist you chose, which makes it quicker to download several songs into the same place.

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

### Data backup
See [Backing up your data](#12-backing-up-your-data).

### Music files
- **Save edits into music files** (on by default) writes edited title, artist, album, category and saved lyrics into the MP3/FLAC file. When it's off, edits stay in Music Tango only. Tags already in a file are still read when you add it. See [Edits are saved into the music file](#edits-are-saved-into-the-music-file).

### Lyrics
- **Lyrics storage folder:** where lyric files are kept. **Use default** keeps them inside the app.
- **Default lyrics font size**
- **Clear Cache** deletes saved lyrics so they are downloaded again.
- **Lyrics generation models:** download or delete the Fun-ASR model used by [Generate lyrics with AI](#generating-lyrics-with-ai). Shown only on 64-bit phones.

### Cover art
- **Cover cache folder:** where downloaded cover images are kept. The default app folder is deleted when you uninstall the app. Choose another folder if you want to keep the covers.

### Radio
- **Radio visual:** **Audio wave** or **Classic radio** on the radio Now Playing screen.
- **Follow the real audio:** when on, the visual moves with the sound. When off, it plays a decorative animation that uses a little less battery.

### Transcription
- **Whisper model file / Download models:** see [Live radio transcription](#9-live-radio-transcription).
- **Radio subtitle delay** shifts subtitles so they line up with the audio.

### About
- **Version** shows the app version you have installed.
- **User manual** opens this manual inside the app, in the app's language. It works offline.

---

## 12. Backing up your data

Go to **Settings → Data backup**.

- **Export data** saves your library, playlists, lyrics cache, download history and radio stations to a file you choose.
- **Import data** restores from a backup file.

> **Warning:** Importing a backup *replaces* all current app data on the device.

Backups contain the app's records, not the audio files themselves. If you restore on a different phone, the songs must also be on that phone. Because edits and lyrics are also saved into MP3 and FLAC files, those songs keep them even without a backup.

---

## 13. Troubleshooting

| Problem | What to try |
|---------|-------------|
| No songs found when scanning | Check that Music Tango has the music/audio permission in Android Settings → Apps. Try **Choose folder** and pick the folder directly. |
| Wrong or missing lyrics | Use **Generate lyrics with AI…**, **Import LRC file…** or **Enter lyrics…**. Check that the song's title and artist are correct with **Edit metadata**. |
| Generated lyrics are inaccurate | Sung vocals are hard to recognize. Try a larger Whisper model, or Fun-ASR for Chinese songs, then fix the rest in the lyrics editor. |
| Lyrics are out of time with the song | Open **Edit lyrics…** and use **Sync line**, **Shift lines…** or **Re-time with AI…**. |
| "Saved in MusicTango only…" after an edit | The file couldn't be changed: permission was declined, the file is read-only, or its tags can't be updated safely. The edit still works in the app. |
| "Fun-ASR needs a 64-bit device" | Fun-ASR can't run on this phone. Use a Whisper model instead. |
| Radio station won't play | The stream may be offline or the URL may have changed. Search for the station again in **Search radio stations**. |
| "Select a Whisper model file in Settings…" | Download and **Use** a model under **Settings → Transcription → Download models**. |
| "Unable to load Whisper model" | The file may be incomplete or not a Whisper GGML/GGUF model. Delete it and download it again, or try a smaller model. |
| "Offline transcription is unavailable…" | Your device may not support the model. Try a smaller model, such as **Tiny**. |
| Subtitles stop with the screen off | This is expected. Turn the screen on to resume. |
| Subtitles out of sync | Adjust **Radio subtitle delay** in Settings. |
| Download fails | Try a different **Source** or a lower **Bitrate**. Check that the download folder is still accessible, and choose it again if needed. |
| Playback controls missing from the notification | Allow notifications for Music Tango in Android Settings. |

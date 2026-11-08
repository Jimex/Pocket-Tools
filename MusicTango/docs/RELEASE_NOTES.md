# Music Tango Release Notes

## 1.0.1.2 (versionCode 1012) · 2026-11-08

[English](#english) · [简体中文](#简体中文) · [繁體中文](#繁體中文) · [Store "What's new" text](#store-whats-new-text)

---

### English

#### Highlights

- **Generate lyrics with AI.** Music Tango can listen to a song and write timed LRC lyrics for it, entirely on your phone. Choose a Whisper model, or download Fun-ASR, which is much better at sung lyrics and at Chinese dialects such as Cantonese.
- **A new lyrics editor.** Edit lyrics full-screen: tap **Sync line** as each line starts, nudge times by 0.1 s, shift many lines at once, drag line markers on a waveform, and let AI re-time the lines you already have. A review list points out missing, out-of-order or duplicate lines before you save. Undo and redo are supported.
- **Your edits are saved into the music file.** Title, artist, album, category and saved lyrics are written into MP3 and FLAC files, so they come back after a reinstall. You can turn this off in **Settings → Music files**.
- **A new radio Now Playing screen.** Radio stations get an **Audio wave** or **Classic radio** visual that moves with the sound, **Previous station** / **Next station** buttons, and a button to turn live subtitles on or off without leaving the screen.

#### Library

- Give songs a **category** with **Edit metadata**, then filter the Home list by category.
- The new **Recently added** filter shows your newest songs first, with the date each was added.
- Tags and lyrics already stored in a file are read when you add it to the library.

#### Lyrics

- **Generate lyrics with AI…** is in the lyrics page's **Lyrics options** (⋮) menu, together with **Import LRC file…**, **Edit lyrics…** and **Text size…**.
- Pick the model and language, or **Auto-detect**. Cantonese is supported. The app remembers your choice.
- Generating new lyrics moves the old lyrics file to an archive folder instead of deleting it.
- Lyrics follow a song when you edit its title, artist or album.

#### Radio

- The radio visual can follow the real audio, or play a lighter decorative animation (**Settings → Radio**).
- When live transcription is off, tap the subtitle area on Now Playing, or **Turn on live transcription** on the transcript page.
- Radio with live subtitles now pauses when another app plays sound, during phone calls, and when headphones are unplugged.

#### Downloads

- **Preview** a result in the API Downloader before downloading it.
- The **Save as** dialog can set a **Category** and add the song to a playlist, and remembers your last choice.

#### Settings

- The new **About** section shows the app version and opens the **User manual** inside the app, in your language, even offline.

#### Fixes

- Fixed a crash when Whisper output contained a Chinese, Japanese or Korean character split across recognition tokens.
- Downloaded songs without tags no longer get "Unknown" as the artist and "Downloaded" as the album. They show the usual placeholder instead.
- Removed the unused microphone (`RECORD_AUDIO`) permission.

#### Upgrade notes

- Your library database is upgraded automatically the first time you open this version. Nothing is lost.
- On Android 10 and later, the app may ask permission the first time it saves an edit into a music file. On Android 9 and earlier it asks for storage write access.
- Fun-ASR is an optional download of about 1.26 GB (plus about 1.5 GB prepared on first use) and needs a 64-bit phone.

---

### 简体中文

#### 主要更新

- **用 AI 生成歌词。** Music Tango 可以听歌并生成带时间的 LRC 歌词，整个过程在手机上完成。可以选择 Whisper 模型，也可以下载 Fun-ASR，它对演唱歌词和粤语等中文方言的识别效果好得多。
- **全新歌词编辑器。** 全屏编辑歌词：在每行开始时点按**同步此行**，以 0.1 秒为单位微调时间，一次平移多行，在波形上拖动歌词标记，还可以让 AI 为现有歌词重新对时。保存前会列出缺少时间、顺序错乱或重复的行。支持撤销和重做。
- **编辑内容会写入音乐文件。** 歌曲名、艺人、专辑、分类和保存的歌词会写入 MP3 和 FLAC 文件，重新安装应用后也能恢复。可以在**设置 → 音乐文件**中关闭。
- **全新的电台“正在播放”界面。** 电台会显示随声音变化的**音频波形**或**复古收音机**动画，提供**上一个电台** / **下一个电台**按钮，并可在当前界面直接开关实时字幕。

#### 曲库

- 用**编辑元数据**为歌曲设置**分类**，然后在首页按分类筛选。
- 新增**最近添加**筛选，最新加入的歌曲排在前面，并显示添加日期。
- 添加歌曲时，会读取文件中已有的标签和歌词。

#### 歌词

- **用 AI 生成歌词…**位于歌词页面的**歌词选项**（⋮）菜单中，同一菜单还有**导入 LRC 文件…**、**编辑歌词…**和**字号…**。
- 可以选择模型和语言，或选择**自动检测**。支持粤语。应用会记住你的选择。
- 生成新歌词时，旧的歌词文件会被移到存档文件夹，而不是删除。
- 修改歌曲名、艺人或专辑后，歌词会跟随歌曲。

#### 电台

- 电台动画可以跟随实际音频，也可以播放更省电的装饰性动画（**设置 → 电台**）。
- 实时字幕关闭时，可以点按“正在播放”界面上的字幕区域，或在字幕记录页面点按**开启实时字幕**。
- 带实时字幕的电台现在会在其他应用播放声音、接听电话或拔出耳机时暂停。

#### 下载

- 在 API 下载器中，下载前可以先**试听**。
- **另存为**对话框可以设置**分类**并把歌曲加入播放列表，还会记住上次的选择。

#### 设置

- 新增**关于**部分，显示应用版本，并可在应用内以你的语言打开**用户手册**，无需联网。

#### 问题修复

- 修复了 Whisper 识别结果中的中文、日文或韩文字符被拆分到不同识别片段时导致的崩溃。
- 没有标签的下载歌曲不再把艺人显示为“Unknown”、专辑显示为“Downloaded”，而是显示通常的占位文字。
- 移除了未使用的麦克风（`RECORD_AUDIO`）权限。

#### 升级说明

- 首次打开此版本时，曲库数据库会自动升级，数据不会丢失。
- 在 Android 10 及以上版本中，应用首次把编辑内容写入音乐文件时可能会请你授权；在 Android 9 及以下版本中，会请求存储写入权限。
- Fun-ASR 为可选下载，约 1.26 GB（首次使用时还会额外准备约 1.5 GB），需要 64 位手机。

---

### 繁體中文

#### 主要更新

- **用 AI 產生歌詞。** Music Tango 可以聽歌並產生帶有時間的 LRC 歌詞，整個過程在手機上完成。可以選擇 Whisper 模型，也可以下載 Fun-ASR，它對演唱歌詞和粵語等中文方言的辨識效果好得多。
- **全新歌詞編輯器。** 全螢幕編輯歌詞：在每行開始時輕觸**同步此行**，以 0.1 秒為單位微調時間，一次平移多行，在波形上拖曳歌詞標記，還可以讓 AI 為現有歌詞重新對時。儲存前會列出缺少時間、順序錯亂或重複的行。支援復原和重做。
- **編輯內容會寫入音樂檔案。** 歌曲名稱、藝人、專輯、分類和儲存的歌詞會寫入 MP3 和 FLAC 檔案，重新安裝應用程式後也能恢復。可以在**設定 → 音樂檔案**中關閉。
- **全新的電台「正在播放」畫面。** 電台會顯示隨聲音變化的**音訊波形**或**復古收音機**動畫，提供**上一個電台** / **下一個電台**按鈕，並可在目前畫面直接開關即時字幕。

#### 曲庫

- 用**編輯中繼資料**為歌曲設定**分類**，然後在首頁依分類篩選。
- 新增**最近新增**篩選，最新加入的歌曲排在前面，並顯示新增日期。
- 加入歌曲時，會讀取檔案中已有的標籤和歌詞。

#### 歌詞

- **用 AI 產生歌詞…**位於歌詞頁面的**歌詞選項**（⋮）選單中，同一選單還有**匯入 LRC 檔案…**、**編輯歌詞…**和**字型大小…**。
- 可以選擇模型和語言，或選擇**自動偵測**。支援粵語。應用程式會記住你的選擇。
- 產生新歌詞時，舊的歌詞檔案會被移到封存資料夾，而不是刪除。
- 修改歌曲名稱、藝人或專輯後，歌詞會跟著歌曲走。

#### 電台

- 電台動畫可以跟隨實際音訊，也可以播放更省電的裝飾性動畫（**設定 → 電台**）。
- 即時字幕關閉時，可以輕觸「正在播放」畫面上的字幕區域，或在字幕紀錄頁面輕觸**開啟實時字幕**。
- 帶即時字幕的電台現在會在其他應用程式播放聲音、接聽電話或拔除耳機時暫停。

#### 下載

- 在 API 下載器中，下載前可以先**試聽**。
- **另存為**對話框可以設定**分類**並把歌曲加入播放清單，還會記住上次的選擇。

#### 設定

- 新增**關於**部分，顯示應用程式版本，並可在應用程式內以你的語言開啟**使用者手冊**，無需連網。

#### 問題修正

- 修正了 Whisper 辨識結果中的中文、日文或韓文字元被拆分到不同辨識片段時導致的當機。
- 沒有標籤的下載歌曲不再把藝人顯示為「Unknown」、專輯顯示為「Downloaded」，而是顯示一般的預留文字。
- 移除了未使用的麥克風（`RECORD_AUDIO`）權限。

#### 升級說明

- 第一次開啟此版本時，曲庫資料庫會自動升級，資料不會遺失。
- 在 Android 10 及以上版本中，應用程式第一次把編輯內容寫入音樂檔案時可能會請你授權；在 Android 9 及以下版本中，會要求儲存空間寫入權限。
- Fun-ASR 為選用下載，約 1.26 GB（首次使用時還會額外準備約 1.5 GB），需要 64 位元手機。

---

### Store "What's new" text

Short versions for the store listing, each under Google Play's 500-character limit. They can be pasted as-is into the Play Console release notes field.

```
<en-US>
• Generate lyrics on your phone with AI (Whisper or Fun-ASR)
• New full-screen lyrics editor: tap-to-sync, waveform, AI re-timing
• Edits and lyrics are saved into MP3/FLAC files and survive a reinstall
• Song categories and a Recently added filter
• Preview songs before downloading
• Radio: new visuals, previous/next station, and live subtitles on/off from Now Playing
• Radio pauses for calls and other apps
• Bug fixes, and the microphone permission is no longer needed
</en-US>
<zh-CN>
• 用 AI 在手机上生成歌词（Whisper 或 Fun-ASR）
• 全新全屏歌词编辑器：点按同步、波形、AI 重新对时
• 编辑内容和歌词会写入 MP3/FLAC 文件，重装后不丢失
• 歌曲分类和“最近添加”筛选
• 下载前可试听
• 电台：新动画、上一个/下一个电台，在“正在播放”界面直接开关实时字幕
• 来电或其他应用播放声音时，电台会自动暂停
• 问题修复，并且不再需要麦克风权限
</zh-CN>
<zh-TW>
• 用 AI 在手機上產生歌詞（Whisper 或 Fun-ASR）
• 全新全螢幕歌詞編輯器：輕觸同步、波形、AI 重新對時
• 編輯內容和歌詞會寫入 MP3/FLAC 檔案，重新安裝後不會遺失
• 歌曲分類和「最近新增」篩選
• 下載前可試聽
• 電台：新動畫、上一個/下一個電台，在「正在播放」畫面直接開關即時字幕
• 來電或其他應用程式播放聲音時，電台會自動暫停
• 問題修正，並且不再需要麥克風權限
</zh-TW>
```

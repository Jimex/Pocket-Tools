# Tango Board — User Manual

**English | [中文](user-manual.zh-CN.md)**

This manual covers installing, enabling, and using Tango Board (the Tango
keyboard). For technical/architecture documentation, see
[ARCHITECTURE.md](ARCHITECTURE.md).

## Contents

- [Installation](#installation)
- [The keyboard at a glance](#the-keyboard-at-a-glance)
- [Switching input modes](#switching-input-modes)
- [English input](#english-input)
- [Pinyin input](#pinyin-input)
- [Wubi input](#wubi-input)
- [Mixed Pinyin + Wubi input](#mixed-pinyin--wubi-input)
- [Symbols, numbers, and emoji](#symbols-numbers-and-emoji)
- [Custom phrases](#custom-phrases)
- [Imported dictionaries](#imported-dictionaries)
- [Learning and suggestions](#learning-and-suggestions)
- [AI writing tools](#ai-writing-tools)
- [Appearance and layout](#appearance-and-layout)
- [Privacy](#privacy)
- [Troubleshooting](#troubleshooting)

## Installation

1. Install the Tango Board app (APK, or from an app store once published).
2. Open the **Tango Board** app. If the keyboard isn't enabled yet, a card at
   the top of the settings screen says **Tango Board is not enabled yet** —
   tap **Enable in system settings** and turn on **Tango Board**.
   - You can also get there yourself: **Settings → System → Languages &
     input → On-screen keyboard → Manage keyboards** (the exact path varies
     by manufacturer).
3. Android shows a warning that a keyboard can read the text you type. This
   is standard for every keyboard app; review it and confirm.
4. Back in the app, if the card now says **Tango Board is not your current
   keyboard**, tap **Switch keyboard** and pick **Tango Board**. You can
   also switch at any time with the keyboard icon in the navigation bar.

## The keyboard at a glance

The strip above the keys (the candidate bar) shows suggestions while you
type. When there is nothing to suggest, it shows tool buttons instead:

| Button | What it does |
|---|---|
| ☰ **Keyboard functions** | Opens the keyboard menu: AI Composer (when AI is enabled), Emoji, Custom phrase, Keyboard height, One-handed, Settings. |
| ✨ **Writing tools** | Opens the AI writing panel (only when AI writing is enabled). |
| 📋 **Paste** | Pastes the current clipboard text. |
| **简 / 繁** | In Chinese modes, switches candidates between Simplified and Traditional. It shows the script currently in use. |
| ⚙ **Settings** | Opens Tango Board settings. |

While suggestions are showing:

- **⌄ Show all candidates** expands the bar into a scrollable grid.
- **✕ Stop suggesting** hides predictions until you type again.

## Switching input modes

- **中/英 key** (next to `123`) — tap to toggle between English and your
  preferred Chinese input (Pinyin by default).
- **Long-press 中/英** to jump straight to English, Pinyin, or Wubi.
- **Settings → Languages → Input modes** controls which modes the key can
  reach (English is always available), and **Preferred Chinese input**
  chooses whether a tap goes to Pinyin or Wubi.
- **简/繁** — use the 简/繁 button on the candidate bar, or set
  **Settings → Languages → Characters** to Simplified, Traditional, or Both.

## English input

Type normally on the QWERTY layout:

- The candidate bar shows completions and corrections as you type — for
  example `wor` may suggest `world`, `word`, `work`. Tap one to replace what
  you typed.
- Space commits exactly what you typed. Tango Board does **not** silently
  autocorrect on space; corrections are offered as candidates for you to
  pick.
- After a word, the bar suggests likely next words.
- **Shift**: tap once for one capital letter, tap again for Caps Lock, and
  tap a third time to turn it off.

## Pinyin input

Type the Pinyin for what you want to say; the composing text appears above
the keyboard and the candidate bar shows characters, words, and phrases.

```text
Type:  nihao
See:   你好 | 您好 | 你号
```

- Tap a candidate to commit it. Words, phrases, and whole sentences commit
  as one unit.
- No tones are needed.
- Long input such as `zhongguoren` is segmented and composed into a sentence
  (`中国人`) as you keep typing.
- **Fuzzy Pinyin** — in **Settings → Languages → Fuzzy pinyin**, turn on
  any pair you want treated as interchangeable. All are off by default.
  - At the start of a syllable: `z/zh`, `c/ch`, `s/sh`, `n/l`, `f/h`, `l/r`
  - At the end of a syllable: `an/ang`, `en/eng`, `in/ing`, `ian/iang`,
    `uan/uang`
- Punctuation switches to full-width Chinese forms (`，。？！：` and curly
  quotes) automatically. A `.` right after a digit stays a decimal point, so
  `3.14` types correctly.

## Wubi input

Select Wubi (long-press 中/英, or set it as **Preferred Chinese input**) and
type a Wubi code; the candidate bar shows matching characters and words.

- **一级简码 (single-key shortcuts)** — the 25 most common characters are one
  keystroke away.
- **Exact codes first** — a code you type in full always lists its own
  characters before longer codes that merely start with it, even if you use
  the longer one more often. Learning and context only reorder candidates
  *within* those two groups. (For example, `bn` always offers 也 before 了.)
- **码满上屏 (auto-commit on a full code)** — when the fourth key completes a
  code that has a candidate, the top candidate is committed automatically.
  An unrecognized four-letter code is never committed as text.
- **`z` reverse lookup** — start with `z` and type Pinyin to find a
  character you can't code; each candidate shows its Wubi code, which is
  handy while learning.
- **`z` wildcard (万能键)** — a `z` after the first key stands for a radical
  position you're unsure of (up to two wildcards).
- **简入繁出 (Simplified input, Traditional output)** — with Traditional
  selected, type the usual Simplified Wubi codes and get Traditional output.

## Mixed Pinyin + Wubi input

With **Settings → Languages → Mixed 拼音/五笔 input** on (the default), the
keyboard also suggests candidates from the other Chinese engine — a plain
Pinyin syllable while typing Wubi, or a Wubi code while typing Pinyin —
ranked below the current mode's own matches.

> Finishing one character via Wubi and the next via Pinyin inside the same
> continuous buffer is not yet supported — see [STATUS.md](STATUS.md).

## Symbols, numbers, and emoji

- **Long-press a letter** to type the small hint shown on it (digits on the
  top row, `!@#$%&*()` on the middle row, `'/-_:;?` on the bottom row).
  With the number row turned on, the top-row hints change to other symbols.
- **Flick up** on a key to type its hint without waiting (can be turned off
  under **Settings → Typing → Flick up for symbols**).
- **Long-press `.`** for `! ? : ; ' "`.
- **`123`** opens the symbols page; **`=\<`** opens more symbols (currency,
  math, `©®™✓`, brackets); **`ABC`** returns to letters.
- **Emoji** — open ☰ → **Emoji**, or long-press `,`. Emoji are grouped by
  category with a **Recent** tab.
- **Number pad** — in number and phone fields, a calculator-style number
  pad (or a phone dialpad) appears automatically. Turn this off under
  **Settings → Typing → Use Number Pad for Numeric Input**.

## Custom phrases

Add your own words, names, or shortcuts, typeable immediately:

- From the keyboard: ☰ → **Custom phrase**.
- From settings: **Settings → Languages → My 词组**.

Enter the phrase and the code you'll type. The code is suggested from the
characters (Pinyin or Wubi — pick under **Code type**); edit it freely. A
short code turns the phrase into a shortcut, and 多音字 may need correcting.
Custom phrases are offered above the built-in dictionary.

## Imported dictionaries

Import a word list to add domain vocabulary in bulk.

1. Go to **Settings → Languages → Imported dictionaries → Import a
   dictionary** and pick a text file.
2. Each line holds a word, an optional code, and an optional weight,
   separated by a **tab or a comma**. Lines starting with `#` are comments:

   ```text
   # my words
   你好	nihao	1000
   中国	zhongguo	850
   软件	ruanjian
   ```

3. The import runs in the background — you can keep typing. When it
   finishes, the dictionary shows its entry count, or **Failed** with the
   reason. Malformed lines are skipped; the rest is still imported.
4. Each imported dictionary can be switched on/off, given a **Priority**
   (higher wins ties with other dictionaries), or deleted.

## Learning and suggestions

Under **Settings → Typing → Suggestions & learning**:

- **Learn from what you type** (on by default) — words you pick rise in the
  candidate list over time. Learning stays on your device.
- **Forget everything learned** — deletes the record of words you've used.
  It takes effect the next time the keyboard opens and does not touch your
  custom phrases or imported dictionaries.
- Nothing typed in password, PIN, or other sensitive fields is learned.

## AI writing tools

AI writing is **off by default**. Turn it on under **Settings → AI Writing →
Enable writing tools**, then choose **Where rewrites run**:

- **Server** — any OpenAI-compatible API. Set **Endpoint**, **Model** (e.g.
  `gpt-4o-mini` or `qwen2.5:7b`), and **API key** (stored encrypted; local
  servers such as Ollama or LM Studio usually need none). Your draft is sent
  to that server.
- **On device (LiteRT-LM)** — a `.litertlm` or `.task` model file on the
  phone. Use **Choose file…**, or paste a direct download link and tap
  **Download**. Optional **GPU acceleration**, **Reasoning**, and **System
  prompt**. Your draft never leaves the device.
- **On device (llama.cpp)** — a GGUF model file chosen with **Choose
  file…**, with an optional **System prompt**.

On-device models need an arm64 phone and roughly 0.5–2 GB of storage and
memory; they are slower and weaker than a good server.

### Using the writing tools

- Tap ✨ **Writing tools** on the candidate bar. It works on the text already
  in the field; if the field is empty, it uses your clipboard text (shown as
  **From clipboard**).
- For a fresh draft, use ☰ → **AI Composer**: write in the panel, then run
  an action on it.
- Built-in actions: **Proofread**, **Rephrase**, **Friendly**,
  **Professional**, **Elaborate**, **Shorten**, **Emojify**, **→ English**,
  **→ 中文**.
- Results stream in as a preview. Tap **Edit** to change them, turn on
  **Continue from result** to run another action on the result, and tap
  **✓ Use this result** to put it in the field. **Undo rewrite** restores
  your original text.
- **Manage Actions** (in AI Writing settings) chooses which actions appear,
  with drag to reorder and **Restore default order**.
- **Custom prompts** — write your own instruction and it becomes a chip in
  the panel. Each can have a **Label**, and optionally its own **System
  prompt** or **No system prompt**.

The writing tools never appear in password or other sensitive fields.

## Appearance and layout

Under **Settings → Appearance**:

- **App language** — System, English, or 简体中文. Applies to settings right
  away and to the keyboard the next time its process restarts.
- **Theme** — System, Light, Dark, Ocean, or Blossom (applies the next time
  the keyboard opens).
- **Key spacing**, **Row spacing**, **Number row**.
- **One-handed mode** — Off, Left, or Right, with an adjustable width. You
  can also cycle it from ☰ → **One-handed**.

Under **Settings → Typing**: **Vibrate on keypress**, **Long-press delay**,
**Flick up for symbols**, and the number pad option.

**Keyboard height** — ☰ → **Keyboard height**, drag to resize, then
**Done** (or **Reset**).

**Settings → Reset to defaults** restores all settings.

## Privacy

- Typing works fully offline — English, Pinyin, Wubi, learning, custom
  phrases, and imported dictionaries never need a network connection.
- Only AI writing with the **Server** backend sends text anywhere, and only
  when you run an action. On-device backends keep your text on the phone.
- Text typed in password, PIN, or other sensitive fields is never learned,
  logged, or sent to AI.

## Troubleshooting

- **Keyboard doesn't appear** — open the Tango Board app; the status card at
  the top tells you whether it still needs enabling or selecting.
- **The keyboard switched back to another keyboard after an update** — some
  devices reset the default keyboard on reinstall. Select Tango Board again.
- **No suggestions in a browser's address bar or some search fields** — those
  fields ask the system for "no suggestions", which disables prediction
  there for every keyboard. This is expected.
- **Suggestions feel generic after Forget everything learned** — expected;
  ranking rebuilds as you type.
- **App language didn't change on the keyboard** — the keyboard picks it up
  the next time its process restarts (e.g. switch keyboards, or reboot).
- **Writing tools button is missing** — check **Enable writing tools** is on,
  and that you're not in a password/sensitive field.
- **Writing tools show an error** — the message says what to fix: add an
  endpoint, check the API key, wait out a rate limit, check the model file,
  or try a smaller model / a server if the device can't run it.

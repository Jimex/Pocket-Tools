# Tango Keyboard

**English | [中文](README.zh-CN.md)**

Tango Keyboard ("Tango Board") is an offline-first Android input method (IME)
supporting **English**, **Pinyin**, and **Wubi** input, with mixed Pinyin/Wubi
composition, on-device learning, and an optional AI writing assistant.


## Features

- **English input** — QWERTY layout, word completion, edit-distance-1
  correction offered as candidates (no silent autocorrect on space),
  next-word prediction, and frequency/context-based candidate ranking.
- **Pinyin input** — full Pinyin with tone-free sentence composition, 11
  optional fuzzy Pinyin rules (e.g. `z`/`zh`, `n`/`l`, `an`/`ang`),
  简体/繁體 (Simplified/Traditional) switching, and full-width Chinese
  punctuation.
- **Wubi input** — Wubi 86 table lookup, 一级简码 (single-key shortcuts),
  exact codes always ranked ahead of longer ones, 码满上屏 (auto-commit on a
  full code), `z` Pinyin reverse lookup with Wubi annotations, `z` wildcard
  (万能键), and 简入繁出 (Simplified input, Traditional output).
- **Mixed Pinyin + Wubi** — optionally also suggests candidates from the
  other Chinese engine (a Pinyin syllable while typing Wubi, or a Wubi code
  while typing Pinyin), ranked below the current mode's own matches.
- **Custom phrases and dictionaries** — add your own phrases and shortcuts
  (with codes suggested automatically), or import word lists in the
  background; see [docs/user-manual.md](docs/user-manual.md) for the format.
- **On-device learning** — words you pick rise in the candidate list over
  time; learning stays local, can be turned off or cleared, and is
  automatically disabled for password/PIN/sensitive fields.
- **AI writing tools** (off by default) — proofread, rephrase, tone,
  elaborate/shorten, translate, a composer for new drafts, and custom
  prompt actions, with streaming output and undo. Runs against a remote
  OpenAI-compatible endpoint or an on-device model (LiteRT-LM or
  llama.cpp/GGUF), isolated from the core keyboard process.
- **Keyboard comfort** — symbol hints with long-press or flick-up, emoji
  panel, automatic number pad for numeric fields, themes, adjustable height
  and spacing, number row, and one-handed mode.
- **Privacy by design** — the keyboard process (`:ime`) has no networking
  dependency; AI features live in a separate process/module and communicate
  over an explicit IPC boundary. User text is never written to logs.


## User manual

- [English user manual](docs/user-manual.md)
- [中文使用手册](docs/user-manual.zh-CN.md)


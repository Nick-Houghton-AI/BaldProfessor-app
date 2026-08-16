# 📚 Bald Professor

**A free, offline study coach.** Drop a course's material into a folder — PDFs,
slides, Word/notes, photos of handwritten notes — and Bald Professor turns it into
study guides, flashcards, scored quizzes, practice exams, spaced-repetition review,
and a tutor that answers from *your own* files.

**No account, no subscription, no cloud.** It works out of the box with no AI model
at all; add a local model or your own AI assistant when you want richer material.

> This is the download page. Bald Professor is free for personal use — see the
> [license](LICENSE.txt). It is not open source.

## Download

Grab the latest build from the **[Releases](../../releases)** page:

| Platform | File |
|---|---|
| **Windows** (64-bit) | `BaldProfessor-windows.zip` |
| **macOS — Apple Silicon** (M1/M2/M3/M4) | `BaldProfessor-macos-arm64.zip` |
| **macOS — Intel** | `BaldProfessor-macos-x86_64.zip` |

> **Which Mac do I have?** Apple menu ▸ *About This Mac*. If the chip line says
> **Apple M1/M2/M3/M4**, take the Apple Silicon build; if it says **Intel**, take the
> Intel one. They aren't interchangeable — the wrong one fails with
> "Bad CPU type in executable".

Unzip it anywhere (e.g. your Desktop) and keep the folder together — your classes
and settings are saved inside it.

## Setup

**There isn't any.** Unzip, run `BaldProfessor`, drop your course files into a
class, and click Generate. **Quick mode** builds flashcards, a study guide and a
quiz straight from your files with no AI model, no downloads and no account.

Everything else — spaced repetition, adaptive Learn, scored quizzes, search,
analytics — works offline too.

### Want better material? Add an AI (optional)

Quick mode pulls out definitions and key passages, but it can't *explain* things
or write exam-style questions. For that, pick one:

**Option A — a local model (stays on your computer)**

1. Install [Ollama](https://ollama.com).
2. Run `ollama pull gemma3:4b` (~3 GB; handles text *and* photos of handwritten
   notes; comfortable on any 16 GB+ laptop). With 32 GB+, `gemma3:12b` is better —
   set it in Settings.

**Option B — an assistant you already use (Claude Desktop, Claude Code, …)**

Bald Professor works as an **MCP server**: your assistant reads your course files
and writes flashcards, guides and quizzes straight back into the app. Best quality,
nothing to install. Setup takes one config entry — see `Extras/SETUP-MCP.md` in the
download.

> **Privacy:** Quick mode and a local model never send anything anywhere. Option B
> does — your assistant receives whatever files it reads. Both AI options are off
> until you set them up.

Your classes, settings and backups are saved inside the app's own folder, so
moving or copying that folder takes your study data with it.

The app checks your setup (**Tools ▸ Run setup check**) and tells you in plain
language if anything's missing — including whether your chosen model is too big
for your machine's memory.

### A note on security warnings
The app isn't code-signed with a paid certificate, so your system will warn you the
first time. This is expected for independent software; it only happens once.

- **Windows** — SmartScreen shows "Windows protected your PC": click **More info ▸ Run anyway**.
- **macOS** — Gatekeeper says the developer can't be verified: **right-click** (or
  Control-click) `BaldProfessor` ▸ **Open** ▸ **Open**. Double-clicking alone won't
  offer the option. If macOS still blocks it, allow it under
  *System Settings ▸ Privacy & Security*.

## What it does

- **Generate** study guides, flashcards, and quizzes from your files — with or without AI.
- **Review** with spaced repetition (remembers exactly when to show each card).
- **Learn** adaptively — drills what you keep getting wrong.
- **Practice** with scored, timed quizzes and weak-topic tracking.
- **Tutor** — grounded Q&A over your files, citing the exact page/slide/timestamp.
- **Exam prep** — mock exams, study plans, and certification mode.
- Plus Connections across courses, analytics, search, and backups.

## Privacy

**Offline by default.** Out of the box — and with a local model — your class
materials and study data never leave your computer. There's no account, no
telemetry, and no cloud storage; your classes are just folders on your disk.

Two things can send data out, and **both are off until you turn them on**:

- **Connecting an assistant over MCP** — it receives whatever course files it reads.
- **Web fetch** — pulling a public page into a class. Restricted to public
  http/https, blocks private and local addresses, and asks before every fetch.

## Support & feedback

Open an issue on this repo. Bug reports and feature ideas welcome — the source is
private, but I read everything.

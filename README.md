# 📚 Bald Professor

**A free, fully-offline AI study coach.** Drop a course's material into a folder —
PDFs, slides, Word/notes, photos of handwritten notes — and Bald Professor turns
it into study guides, flashcards, scored quizzes, practice exams, spaced-repetition
review, and a tutor that answers from *your own* files. Everything runs on a local
AI model on your computer; **nothing ever leaves your machine.**

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

## Setup (one time, ~5 minutes)

Bald Professor needs a local AI model to run. The recommended one is small, fast,
and free:

1. **Install [Ollama](https://ollama.com)** (Windows or macOS).
2. **Pull the model** — open a terminal and run:
   ```
   ollama pull gemma3:4b
   ```
   Gemma 3 4B is ~3 GB, handles both text and photos of notes, and runs comfortably
   on any 16 GB+ laptop (including Apple silicon). Have 32 GB+ and want more quality?
   Pull `gemma3:12b` and set it in Settings.
3. **Run Bald Professor** — Windows: double-click `BaldProfessor.exe`. macOS: open the
   unzipped folder and run `BaldProfessor` (see the note below on the first launch).
   It opens in its own window. That's it.

Your classes, settings and backups are saved inside the app's own folder, so
moving or copying that folder takes your study data with it.

The app checks your setup on first launch (**Tools ▸ Run setup check**) and tells
you in plain language if anything's missing.

### A note on security warnings
The app isn't code-signed with a paid certificate, so your system will warn you the
first time. This is expected for independent software; it only happens once.

- **Windows** — SmartScreen shows "Windows protected your PC": click **More info ▸ Run anyway**.
- **macOS** — Gatekeeper says the developer can't be verified: **right-click** (or
  Control-click) `BaldProfessor` ▸ **Open** ▸ **Open**. Double-clicking alone won't
  offer the option. If macOS still blocks it, allow it under
  *System Settings ▸ Privacy & Security*.

## What it does

- **Generate** study guides, flashcards, and quizzes from your files.
- **Review** with spaced repetition (remembers exactly when to show each card).
- **Learn** adaptively — drills what you keep getting wrong.
- **Practice** with scored, timed quizzes and weak-topic tracking.
- **Tutor** — grounded Q&A over your files, citing the exact page/slide/timestamp.
- **Exam prep** — mock exams, study plans, and certification mode.
- Plus Connections across courses, analytics, search, and backups.

## Privacy

100% offline by design. Your class materials and study data never leave your
computer. Optional web fetch is off unless you turn it on, and asks before every
fetch.

## Support & feedback

Open an issue on this repo. Bug reports and feature ideas welcome — the source is
private, but I read everything.

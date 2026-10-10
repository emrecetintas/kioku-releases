# Kioku

**Remember what you read.** Kioku is a desktop app for incremental reading and
spaced repetition. Import articles and PDFs, read them a little at a time,
turn what matters into flashcards as you go, and review each card just before
you'd forget it.

It runs on your computer, with no account, and your data stays in files you
own. Free during the beta, for macOS, Windows and Linux.

[kiokuweb.com](https://kiokuweb.com) · [Docs](https://docs.kiokuweb.com) ·
[What's new](https://github.com/emrecetintas/kioku-releases/releases/latest)

This repository holds Kioku's releases, its bug tracker and its discussions.
The app's source code isn't public.

## Download

Open the [latest release](https://github.com/emrecetintas/kioku-releases/releases/latest)
and pick the file for your computer (`<version>` is the release number, such
as `0.6.1`):

| Computer | File |
| --- | --- |
| Mac with Apple silicon (M1 or later) | `Kioku-<version>-mac-arm64.dmg` |
| Mac with an Intel processor | `Kioku-<version>-mac-x64.dmg` |
| Windows (64-bit) | `Kioku-<version>-x64.exe` |
| Linux, any distribution | `Kioku-<version>-x86_64.AppImage` |
| Debian, Ubuntu and their relatives | `Kioku-<version>-amd64.deb` |

`.zip` versions are there too, for macOS (`Kioku-<version>-mac-arm64.zip`,
`Kioku-<version>-mac-x64.zip`) and Windows (`Kioku-<version>-x64.zip`).
Not sure which Mac you have? Apple menu → **About This Mac**: "Apple M…" means
Apple silicon, "Intel" means Intel.

## Installing

**macOS.** Open the `.dmg` and drag **Kioku** into **Applications**, then open
it from there.

**Windows.** Run the installer. Windows may say **"Windows protected your
PC"**, because it doesn't recognize Kioku yet. Choose **More info**, then
**Run anyway**.

**Linux.** Make the AppImage executable, then run it:

```bash
chmod +x Kioku-*.AppImage
./Kioku-*.AppImage
```

Or install the `.deb`:

```bash
sudo apt install ./Kioku-<version>-amd64.deb
```

## Updates

Kioku checks for a new version when it starts, and whenever you choose
**Settings → About → Check for updates**. When there is one, a banner offers
it: Kioku downloads it when you say so and installs it when you restart.
Your collections are backed up before every update.

## What it does

- **Incremental reading.** Import web pages and PDFs, read them in short
  passes, and pull out the passages that matter as extracts. Select text and
  press **X** to extract or **Z** to make a cloze card, without leaving the
  page. Pages can be a snapshot or stay live.
- **Spaced repetition with FSRS-6**, for cards. Reading comes back on its own
  priority schedule.
- **Cards of every kind:** basic, cloze, image occlusion, and audio cloze.
  Add pictures and sound to any card, or record your own.
- **Import from Anki.** Bring `.apkg` decks, including Anki's default export:
  every field from each note type's own templates, cloze **Back Extra**,
  pictures and sound, suspended cards, and each card's progress as an
  approximate FSRS schedule. Tags, review history and card styling stay
  behind. Big decks import in the background.
- **Browse** your collection as a tree, or your cards as a sortable table like
  Anki's Browser (question, where it lives, due date, interval, lapses).
- **An editor that keeps up:** a menu over the selection, **/** for blocks,
  links, pasted and dropped images, and saving you can see.
- **Your data is safe and yours.** Each collection is a local SQLite file. Kioku
  backs it up every 30 minutes and before every update, exports everything to
  a `.zip` in one click, and keeps deleted items in a Trash with Undo.
- **More than one computer?** Kioku has no cloud of its own, but
  [Syncthing](https://docs.kiokuweb.com/guides/sync-between-computers/) keeps
  your collections in step.
- **Plan**, optional: lay out your day as a list of activities and run it with
  a countdown.

## Feedback and help

- **Found a bug?** [Open an issue](https://github.com/emrecetintas/kioku-releases/issues/new/choose).
  In Kioku, **Settings → About → Copy diagnostics** first, and paste it in: it
  has versions and counts, never your notes or cards.
- **Questions and ideas:** the [Discord](https://discord.gg/6Fe26qstTj), or
  [Discussions](https://github.com/emrecetintas/kioku-releases/discussions).
  On Discord, #help and #bugs need no GitHub account.
- **No GitHub account?** Email [kiokufeedback@gmail.com](mailto:kiokufeedback@gmail.com).
- **Beta news by email,** now and then: [sign up](https://kiokuweb.com/#beta-list).
- **How do I…?** The [docs](https://docs.kiokuweb.com) and their
  [FAQ](https://docs.kiokuweb.com/troubleshooting/faq/).

## Supporting Kioku

Kioku is free during the beta, and nothing in it is locked. If it's useful to
you, there's an optional [Ko-fi tip jar](https://ko-fi.com/emrec3); a tip buys
nothing.

## License and privacy

Kioku is proprietary software, free to use during the beta under the
[Kioku Beta License](EULA.md). Your data is not proprietary: collections are
local files in a documented format, export is built in, and no version of
Kioku, free or paid, will ever gate it. If the project is ever discontinued,
the source will be released.

Usage analytics is off unless you turn it on, and never includes what you
read or write. See the [Privacy Policy](https://docs.kiokuweb.com/legal/privacy/).

# Transcriber

Batch audio transcription with Whisper, entirely on your own computer.
Nothing is uploaded and no account is needed. Only the speech model is
downloaded once, the first time it is used.

- Transcribes whole folders of recordings
- Splits long recordings into sections of about ten minutes, cut in a pause,
  and resumes where it stopped if a run is interrupted
- Detects and redoes passages where Whisper gets stuck repeating itself
- Output: text with a timecode at least every 30 seconds (optionally in frames
  from the recording's start timecode), SRT/VTT subtitles and PDF

No Python setup or separate ffmpeg install is needed. The macOS version uses
the Apple GPU; the Windows and Linux packages use faster-whisper and run on the CPU.

> **Downloads are temporarily unavailable.** The 1.1.1 packages did not yet
> include the license texts and source offers required by some bundled
> third-party components. A corrected release will follow.

## Install

Download the file for your system from the [latest release](../../releases/latest).

### macOS (Apple Silicon, M1 and later, macOS 13 or newer)

1. Open `Transcriber-1.1.1-macos-arm64.dmg` and drag Transcriber to Applications.
2. The app is not notarized by Apple, so the first start needs one extra step:
   in Applications, **right-click → Open**, then confirm **Open**. If macOS does
   not offer that: **System Settings → Privacy & Security → "Open Anyway"**.

### Windows (10 and 11, 64-bit)

1. Run `Transcriber-1.1.1-windows-x64-setup.exe`.
2. The installer is not signed. If "Windows protected your PC" appears, click
   **More info → Run anyway**.

### Linux (x86-64)

| System | Command |
|---|---|
| Debian, Ubuntu (22.04 and newer) | `sudo apt install ./whisper-transcriber_1.1.1_amd64.deb` |
| Fedora, openSUSE | `sudo dnf install ./whisper-transcriber-1.1.1-1.x86_64.rpm` |

Start it from the application menu ("Transcriber") or run `whisper-transcriber`.
For the command line, use `whisper-transcriber --cli --help`.

**Why "whisper-transcriber"?** Ubuntu already has an unrelated package called
`transcriber`, so the package and command use this name to stay distinct.

## Known limitations

- It does not tell speakers apart yet.
- If the language changes within a section, the other language comes out
  inaccurate.
- The packages are not signed, and the macOS app is not notarized.
- The Windows version passes the automatic test (it transcribes a test tone),
  but has not yet been tried by hand on a real Windows PC.

## License

MIT, see [LICENSE](LICENSE). Bundled third-party components keep their own
licenses, listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

This repository holds the releases. The source code is not public.

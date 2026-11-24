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

The Linux packages use faster-whisper and run on the CPU. No GPU, Python setup
or separate ffmpeg install is needed.

## Install (Linux, x86-64)

Download the package from the [latest release](../../releases/latest), then:

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
- The packages are not signed.

## License

MIT, see [LICENSE](LICENSE). Bundled third-party components keep their own
licenses, listed in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

This repository holds the releases. The source code is not public.

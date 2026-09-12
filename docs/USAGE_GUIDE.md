# CleanWrap - Usage Guide

## How It Works
CleanWrap organizes files into categories based on extension:

| Category | Extensions |
|----------|-----------|
| Documents | .pdf, .doc, .docx, .txt, .xlsx |
| Images | .jpg, .png, .gif, .svg, .webp |
| Videos | .mp4, .avi, .mkv, .mov |
| Audio | .mp3, .wav, .flac, .aac |
| Archives | .zip, .rar, .7z, .tar.gz |
| Code | .py, .js, .cpp, .java, .html |
| Executables | .exe, .msi, .bat |

## Quick Start
```bash
# Organize current directory
cleanwrap .

# Organize Downloads folder
cleanwrap C:\Users\You\Downloads

# Dry run (preview without moving)
cleanwrap . --dry-run

# Custom categories
cleanwrap . --config custom_rules.json
```

## Performance
| Files | Time |
|-------|------|
| 100 | < 1s |
| 1,000 | ~2s |
| 10,000 | ~8s |

## Safety
- Never overwrites existing files
- Creates undo log for reverting
- Dry-run mode to preview changes
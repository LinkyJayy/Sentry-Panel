# Sentry Panel

> God Mode for Windows!

A sleek dark-themed GUI that gives you instant access to hundreds of hidden Windows settings, shell folders, deep links, and system shortcuts — all in one place.

![Screenshot](panel.png)

## Features

- **7 shortcut categories** — All Task Links, CLSID Shell Folder Shortcuts, Deep Links, Hidden App Links, Special Named Folders, System Settings, URL Protocols
- **Real-time search** — filter shortcuts within the selected category
- **One-click launch** — opens any shortcut via the Windows shell
- **Dark green & purple theme** with responsive card grid

## Quick Start

### Run from source

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python sentry_panel.py
```

### Build standalone exe

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --name "Sentry Panel" --icon=panel.ico ^
  --add-data "panel.png;." --add-data "panel.ico;." --add-data "Recourses;Recourses" ^
  sentry_panel.py
```

The exe will be in the `dist/` folder.

## Requirements

- Windows 10 / 11
- Python 3.10+ (for running from source)

## License

MIT

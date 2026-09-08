<div align="center">

# 🎵 AudioDupSelector

**A simple web interface for sorting audio duplicates detected by `dupsonic.exe`.**

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-required-black?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Languages](https://img.shields.io/badge/Languages-6-green)](#-languages)

Listen to duplicate files, choose which one to keep, and safely move the other one to `trier/`.

**Nothing is permanently deleted.**

[⬇️ Downloads](https://github.com/MATTRAX64/AudioDupSelector/releases) ·
[🐛 Issues](https://github.com/MATTRAX64/AudioDupSelector/issues)

</div>

---

## ✨ Features

- 🎵 Detect duplicates with `dupsonic.exe`
- 🌐 Lightweight local web interface
- ▶️ Listen to files before choosing
- ↩️ Undo a choice
- 📁 Unkept files are moved to `trier/`
- 🛡️ No permanent deletion
- 🌍 Available in **6 languages**

## 🌍 Languages

| Language | |
|---|---|
| 🇫🇷 Français | 🇬🇧 English |
| 🇪🇸 Español | 🇩🇪 Deutsch |
| 🇷🇺 Русский | 🇯🇵 日本語 |

## 📋 Requirements

- **Python**
- **`dupsonic.exe`**
- **Flask**

Install Flask:

```bash
pip install flask
```

## 🚀 Usage

Run the application:

```bash
python AudioDupSelector.pyw
```

A folder selection window will appear. Choose the folder containing your audio files.

### Options

```bash
python AudioDupSelector.pyw --dossier "C:\path\to\audio"
python AudioDupSelector.pyw --exe "C:\path\to\dupsonic.exe"
python AudioDupSelector.pyw --port 8765
python AudioDupSelector.pyw --no-browser
```

## 🔄 How it works

1. `dupsonic.exe` scans the selected audio folder.
2. Audio duplicates are detected.
3. Duplicate pairs are displayed in the web interface.
4. Listen to both files.
5. Click **Keep this one**.
6. The other file is moved to `trier/`.

> [!NOTE]
> Groups containing 3 or more duplicate files are not currently handled by the selection interface.

## 🛡️ Safety

AudioDupSelector does **not permanently delete files**.

When you keep one file, the other is moved to:

```text
trier/
```

This makes it possible to recover a file if you make a mistake.

## 📥 Download

Get the latest version from the **[Releases](https://github.com/MATTRAX64/AudioDupSelector/releases)** page.

## 📄 License

See the main repository for license information.

---

<div align="center">

Made with ❤️ for easier audio library cleanup.

</div>

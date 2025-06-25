<div align="center">

# 🎵 SUPER SPOTIFY Script

<img src="https://user-images.githubusercontent.com/74038190/212257467-871d32b7-e401-42e8-a166-fcfd7baa4c6b.gif" width="100">

[![Shell](https://img.shields.io/badge/Shell-Script-green?style=for-the-badge&logo=gnu-bash&logoColor=white)](https://www.gnu.org/software/bash/)
[![Spotify](https://img.shields.io/badge/Spotify-1ED760?style=for-the-badge&logo=spotify&logoColor=white)](https://spotify.com)
[![Version](https://img.shields.io/badge/Version-6.6.6-blue?style=for-the-badge)](https://github.com/riel-fas/Spotify_script)

*Transform your Spotify experience with powerful modifications*

</div>

---

## 📋 Table of Contents

- [🎯 Overview](#-overview)
- [✨ Features](#-features)
- [🔧 Installation](#-installation)
- [📖 Usage](#-usage)
- [⚙️ Configuration Options](#️-configuration-options)
- [🖥️ Platform Support](#️-platform-support)
- [⚠️ Important Notes](#️-important-notes)

---

## 🎯 Overview

**SUPER SPOTIFY** is a powerful bash script that modifies your Spotify desktop client to unlock premium features, remove advertisements, and enhance your music streaming experience. This script is based on SpotX-Bash technology and supports both macOS and Linux platforms.

---

## ✨ Features

### 🚫 Ad Removal
- **Complete ad blocking** - Remove all audio, visual, and banner advertisements
- **Clean interface** - Hide promotional content and upgrade prompts
- **Seamless experience** - Uninterrupted music playback

### 🎵 Premium Features
- **Unlimited skips** - Skip as many tracks as you want
- **High-quality audio** - Access to better audio quality options
- **Enhanced controls** - Advanced playback controls and features

### 🎨 Interface Enhancements
- **Developer mode** - Access to advanced debugging tools
- **Custom UI options** - Choice between old and new interface designs
- **Hide non-music content** - Focus on music by hiding podcasts and other content
- **Dark lyrics background** - Enhanced lyrics viewing experience

### 🔧 Advanced Options
- **Auto-update blocking** - Prevent unwanted client updates
- **Cache management** - Clear app cache when needed
- **Interactive mode** - Step-by-step configuration wizard
- **Backup system** - Automatic backup and restore functionality

---

## 🔧 Installation

### Prerequisites

<details>
<summary>📋 Required Dependencies</summary>

**All Platforms:**
- `perl` - Text processing
- `unzip` - Archive extraction
- `zip` - Archive creation

**macOS Additional:**
- `codesign` - Code signing (Xcode Command Line Tools)
- macOS 10.11+ required

**Linux Additional:**
- `apt` - Package management (for Debian-based distros)

</details>

### Quick Install

```bash
# Download the script
curl -sSL https://raw.githubusercontent.com/riel-fas/Spotify_script/main/spotx.sh -o spotx.sh

# Make it executable
chmod +x spotx.sh

# Run the script
./spotx.sh
```

### Alternative Methods

<details>
<summary>🐧 Linux (Debian/Ubuntu)</summary>

```bash
# Install latest Spotify client and apply modifications
./spotx.sh --installdeb

# For stable branch
./spotx.sh --installdeb --stable
```

</details>

<details>
<summary>🍎 macOS</summary>

```bash
# Install latest supported Spotify version
./spotx.sh --installmac

# Install specific version
./spotx.sh --installmac -V 1.2.20.1218
```

</details>

---

## 📖 Usage

### Basic Usage

```bash
# Run with default settings
./spotx.sh

# Interactive mode (recommended for first-time users)
./spotx.sh --interactive

# Force run (bypass existing installation checks)
./spotx.sh --force
```

### Advanced Usage Examples

```bash
# Premium user with developer mode and old UI
./spotx.sh --premium --devmode --oldui

# Hide non-music content and clear cache
./spotx.sh --hide --clearcache

# Block updates and enable black lyrics background
./spotx.sh --blockupdates --lyricsbg

# Custom installation path
./spotx.sh -P /custom/path/to/spotify
```

---

## ⚙️ Configuration Options

<div align="center">

| Option | Short | Description |
|--------|-------|-------------|
| `--blockupdates` | `-B` | 🚫 Block automatic client updates (macOS) |
| `--clearcache` | `-c` | 🧹 Clear application cache |
| `--devmode` | `-d` | 🔧 Enable developer mode |
| `--noexp` | `-e` | ❌ Exclude experimental features |
| `--force` | `-f` | ⚡ Force script execution |
| `--hide` | `-h` | 👁️ Hide non-music content on home |
| `--interactive` | `-i` | 🎮 Enable interactive configuration |
| `--lyricsbg` | `-l` | 🎤 Black lyrics background |
| `--oldui` | `-o` | 🕰️ Use classic interface |
| `--premium` | `-p` | 💎 Premium subscriber mode |
| `--skipcodesign` | `-S` | ✍️ Skip code signing (macOS) |
| `--uninstall` | | 🔄 Uninstall modifications |
| `--version` | `-v` | ℹ️ Show version information |

</div>

---

## 🖥️ Platform Support

<div align="center">

### Supported Platforms

| Platform | Status | Architecture | Notes |
|----------|--------|--------------|-------|
| 🍎 **macOS** | ✅ Full Support | Intel & Apple Silicon | Requires macOS 10.11+ |
| 🐧 **Linux** | ✅ Full Support | x86_64 | Debian/Ubuntu recommended |

### Spotify Client Versions

| Version Range | Support Status | Features |
|---------------|----------------|----------|
| `1.1.59.710+` | ✅ Full Support | All features available |
| `1.2.x.x` | ✅ Latest Support | Enhanced features |
| `< 1.1.59.710` | ❌ Unsupported | Too old |

</div>

---

## ⚠️ Important Notes

<div align="center">
<img src="https://user-images.githubusercontent.com/74038190/216644497-1951db19-8f3d-4e44-ac08-8e9d7e0d94a7.gif" width="100">
</div>

### 🛠️ Technical Considerations

- **Backup system** - Script automatically creates backups before modification
- **Reversible** - Use `--uninstall` to restore original client
- **Updates** - Spotify updates may break modifications
- **Permissions** - May require sudo access for system-wide installations

### 💡 Troubleshooting

<details>
<summary>Common Issues & Solutions</summary>

**Script fails to run:**
```bash
# Check permissions
chmod +x spotx.sh

# Install missing dependencies
# macOS: xcode-select --install
# Linux: sudo apt install perl unzip zip
```

**Spotify won't start:**
```bash
# Restore from backup
./spotx.sh --uninstall

# Clear cache and retry
./spotx.sh --clearcache --force
```

**Modifications not working:**
```bash
# Force reinstall
./spotx.sh --force

# Check Spotify version
./spotx.sh --version
```


---

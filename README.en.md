# APM — Android Package Manager

<p align="center">English | <a href="README.md">简体中文</a></p>

**APM** is a cross-platform desktop application for Android APK packaging, signing, and project management. Built with [Wails](https://wails.io) (Go) + React + TypeScript, it's lightweight (≈8MB) and fast.

## ✨ Features

### 📊 Dashboard
Overview of projects, SDK status, and quick actions.

![Dashboard](Samples/dashboard.png)

### 📁 Project Management
Import existing Android projects or create new ones from templates (Empty Activity, Jetpack Compose, Library Module).

| Project List | New Project |
|:---:|:---:|
| ![Projects](Samples/projects.png) | ![New Project](Samples/new.png) |

### 🔨 Build & Package
Configure build variants (debug/release/AAB), set JAVA_HOME, pass extra Gradle arguments, and watch real-time build output — all in one place.

![Build](Samples/build.png)

### ⚙️ Gradle Management
- View all locally cached Gradle versions
- Upgrade the Gradle Wrapper for any project
- Delete outdated versions to reclaim disk space

![Gradle](Samples/gradle.png)

### 📱 Android SDK Management
Check installed platforms and build-tools at a glance, explore available versions to download.

![SDK](Samples/SDK.png)

### 🔐 APK Signing
- List and select keystores (debug / release)
- Sign APK files with `apksigner`
- Verify existing signatures
- Create a debug keystore in one click

![Signing](Samples/key.png)

### 🔍 APK Analyzer
Select an APK and instantly see:
- Package name, version name/code, SDK targets
- Declared permissions and features
- Signature verification status

![Analyzer](Samples/analyze.png)

---

## 🚀 Installation

### Download Pre-built Binary

| Platform | Architecture | Format |
|----------|-------------|--------|
| macOS    | arm64 / x64 | `.app` / `.dmg` |
| Windows  | x64         | `.exe` installer |
| Linux    | x64         | `.AppImage` / `.deb` |

> 💡 Pre-built binaries will be available from the [Releases](https://github.com/your-username/apm/releases) page.

### System Requirements

| Component | Required |
|-----------|----------|
| Operating System | macOS 12+, Windows 10+, Linux (GTK3) |
| Android SDK | `ANDROID_HOME` environment variable set |
| Java | JDK 17+ (for Gradle builds and APK signing) |
| AAPT | Included with Android SDK Build-Tools |

---

### Tech Stack

| Layer | Technology |
|-------|-----------|
| Desktop Shell | [Wails v2](https://wails.io) |
| Backend | Go 1.26 |
| Frontend | React 19, TypeScript, Vite 8 |
| Styling | Tailwind CSS 3 |
| Icons | Lucide React |
| State | Zustand |
| APK parsing | Android SDK `aapt` + `apksigner` |

---

## 📄 License

MIT

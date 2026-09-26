<p align="center">
  <img src="assets/buildly.png" width="96" height="96" alt="Buildly">
</p>

<h1 align="center">Buildly</h1>

<p align="center">
  Your local dev dashboard: create, run and maintain all your projects, with Git, Docker, databases and the tools they need, in one app.
</p>

<p align="center">
  <strong>Version 0.2.1</strong> · released September 26, 2026 · Windows, macOS and Linux
</p>

## Download

| System | Download |
| --- | --- |
| **Windows** 10, 11 | [![Windows Installer (.exe)](https://img.shields.io/badge/Windows-Installer_%28.exe%29-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_x64-setup.exe)<br><sub>or the [.msi package](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_x64_en-US.msi)</sub> |
| **macOS** 11 or newer | [![macOS Apple Silicon](https://img.shields.io/badge/macOS-Apple_Silicon-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_aarch64.dmg) [![macOS Intel](https://img.shields.io/badge/macOS-Intel-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_x64.dmg) |
| **Linux** | [![Linux AppImage](https://img.shields.io/badge/Linux-AppImage-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_amd64.AppImage) [![Linux .deb](https://img.shields.io/badge/Linux-.deb-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly_0.2.1_amd64.deb) [![Linux .rpm](https://img.shields.io/badge/Linux-.rpm-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.2.1/Buildly-0.2.1-1.x86_64.rpm) |

Buildly updates itself: new versions show up in the app, and one click installs them. Older versions and all files are on the [releases page](https://github.com/B3nd4b0ss/Buildly_Release/releases).

## What Buildly does

- **All your projects in one place.** Every folder in your workspace shows up with its stack (Spring Boot, React, Django, Go, .NET…), Git status and last change. Pin favorites, search and filter.
- **New projects in seconds.** About 27 templates: Spring Boot, Maven, Gradle, React, Vue, Svelte, Next.js, Angular, Express, NestJS, FastAPI, Flask, Django, ASP.NET Core, Go, Rust, PHP and more, with Git, a GitHub repository and a database if you like.
- **Run and watch.** Start dev servers, scripts and build tasks with live output and clickable local URLs. They keep running when you close Buildly and are back under your control when you open it again.
- **Git without the terminal.** Changes with diffs, commit and push, pull, branches, history, and new GitHub repositories.
- **Docker.** Containers with live CPU and memory, logs, shell, compose projects, images and volumes. Create containers from an image, a Dockerfile, a compose file or a script.
- **Databases.** PostgreSQL, MySQL, MariaDB, MongoDB and Redis in Docker, plus SQLite: create them with a starter schema, browse tables, run queries, and connect them to a project (`.env`, driver and framework config included).
- **Tools.** See which languages and tools are installed (Node.js, Python, Java, Maven, Gradle, Go, Rust, .NET, PHP, Git, Docker…) and install or update them with one click.
- **Logs.** Buildly keeps a log of what it does, so problems can be looked at afterwards.

Everything runs on your computer. Buildly only listens on `127.0.0.1` and keeps its settings in `~/.buildly`.

## What's new in 0.2.1

- fixed path of downloading tools added version controlls for tools
- added ticketing system

## Installing

**Windows 10 or 11:** run the installer; no administrator rights needed. Windows may show "Windows protected your PC" because the app is not code-signed yet: click **More info → Run anyway**.

**macOS 11 or newer:** open the `.dmg` and drag Buildly into Applications. The app is not notarized yet, so the first start is blocked: right-click Buildly in Applications and choose **Open**, or run:

```bash
xattr -dr com.apple.quarantine /Applications/Buildly.app
```

**Linux:** the AppImage runs on most distributions and updates itself:

```bash
chmod +x Buildly_*.AppImage && ./Buildly_*.AppImage
```

Or install the package: `sudo apt install ./Buildly_*.deb` (Debian, Ubuntu) or `sudo dnf install ./Buildly-*.rpm` (Fedora). Packages are updated by installing the new version.

Buildly uses the tools already on your computer: Git, and Docker for containers and databases. Anything missing can be installed from its **Tools** page.

<p align="center">
  <img src="assets/buildly.png" width="96" height="96" alt="Buildly">
</p>

<h1 align="center">Buildly</h1>

<p align="center">
  Your local dev dashboard: create, run and maintain all your projects, with Git, Docker, databases and the tools they need, in one app.
</p>

<p align="center">
  <strong>Version 0.3.2</strong> · released October 31, 2026 · Windows, macOS and Linux
</p>

## Download

| System | Download |
| --- | --- |
| **Windows** 10, 11 | [![Windows Installer (.exe)](https://img.shields.io/badge/Windows-Installer_%28.exe%29-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_x64-setup.exe)<br><sub>or the [.msi package](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_x64_en-US.msi)</sub> |
| **macOS** 11 or newer | [![macOS Apple Silicon](https://img.shields.io/badge/macOS-Apple_Silicon-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_aarch64.dmg) [![macOS Intel](https://img.shields.io/badge/macOS-Intel-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_x64.dmg) |
| **Linux** | [![Linux AppImage](https://img.shields.io/badge/Linux-AppImage-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_amd64.AppImage) [![Linux .deb](https://img.shields.io/badge/Linux-.deb-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly_0.3.2_amd64.deb) [![Linux .rpm](https://img.shields.io/badge/Linux-.rpm-8B7CFF?style=for-the-badge)](https://github.com/B3nd4b0ss/Buildly_Release/releases/download/v0.3.2/Buildly-0.3.2-1.x86_64.rpm) |

Buildly updates itself: new versions show up in the app, and one click installs them. Older versions and all files are on the [releases page](https://github.com/B3nd4b0ss/Buildly_Release/releases).

## What Buildly does

- **All your projects in one place.** Every folder in your workspace shows up with its stack (Spring Boot, React, Django, Go, .NET…), Git status and last change. Pin favorites, search and filter.
- **New projects in seconds.** About 27 templates: Spring Boot, Maven, Gradle, React, Vue, Svelte, Next.js, Angular, Express, NestJS, FastAPI, Flask, Django, ASP.NET Core, Go, Rust, PHP and more, with Git, a GitHub repository and a database if you like.
- **Run and watch.** Start dev servers, scripts and build tasks with live output and clickable local URLs. They keep running when you close Buildly and are back under your control when you open it again.
- **Git without the terminal.** Changes with diffs, commit and push, pull, branches, history, and new GitHub repositories.
- **Docker.** Containers with live CPU and memory, logs, shell, compose projects, images and volumes. Create containers from an image, a Dockerfile, a compose file or a script.
- **Databases.** PostgreSQL, MySQL, MariaDB, MongoDB and Redis in Docker or on your own database servers, plus SQLite: create them with a starter schema, browse tables, run queries, and connect them to a project (`.env`, driver and framework config included).
- **Your own database servers.** Connect the PostgreSQL, MySQL, MariaDB, MongoDB or Redis server you already have, on your computer or elsewhere, and Buildly creates new databases right inside it, each with a user of its own. No Docker needed.
- **Tools.** See which languages and tools are installed (Node.js, Python, Java, Maven, Gradle, Go, Rust, .NET, PHP, Git, Docker…) and install or update them with one click.
- **Logs.** Buildly keeps a log of what it does, so problems can be looked at afterwards.

Everything runs on your computer. Buildly only listens on `127.0.0.1` and keeps its settings in `~/.buildly`.

## What's new in 0.3.2

- Projects deeper inside your folders are found now, not only those right at the top
- A folder that is a Git repository around other projects (like a school folder with a project per module) shows as one project with a new **Projects** tab: every project inside it as a card, with its run button and actions. Pin one of them to also see it on the Projects page.
- Choose for each folder whether its projects show as one project or each on its own: in Settings → Folders with projects, in a project's Settings tab, or from a card's ⋯ menu.
- Shell scripts run with one click: `.sh`, `.ps1`, `.bat` and `.cmd` files in a project (and in folders like `scripts/`) are listed on its Overview and Run tabs and in the ▾ menu of its card. A folder with just scripts in it is a project too. On Windows, `.sh` scripts run with Git Bash, and you can answer their prompts in the terminal.
- Buildly has a tray icon (menu bar icon on macOS): it lists your processes with Start, Stop and Restart, opens Buildly and quits it. Closing the window keeps Buildly in the tray, so notifications keep coming; turn this off in Settings → Desktop app.
- Notifications when a process stops unexpectedly, a build or other task finishes, or the checks of one of your pull requests fail. They show while Buildly is not the window in front; choose which ones in Settings → Notifications. In the browser, allow them there first.
- See what changed: **Release notes** in Settings shows the latest Buildly versions with their notes and marks the one you have.
- GitHub Actions in the Git tab: a new **Actions** view lists the workflow runs of your branch or of all branches, the bar shows whether CI passed for your branch, and History and the pull request list show an icon per commit. A run opens right in Buildly with its jobs, steps and logs (the failed job's log opens by itself, at its first error), and you can re-run failed jobs, re-run everything or cancel a run there.

## Installing

**Windows 10 or 11:** run the installer and accept the terms of use; no administrator rights needed. At the end it asks once whether Buildly may work without asking every time (a Windows Firewall rule for Buildly's Node.js, for which Windows asks for permission, and no confirmation before administrator actions); you can change this later in Settings. Windows may show "Windows protected your PC" because the app is not code-signed yet: click **More info → Run anyway**.

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

# Mike Holp: open source Linux and Windows desktop apps in Rust, Tauri, C++ and Qt

I'm a software developer in Koh Samui, Thailand. I build free, open source desktop apps for Linux and
Windows: a task manager, an app launcher, a backup manager, a text editor, a software updater and a
WireGuard VPN client. I write most of them with AI coding agents such as Claude Code and Codex, and I
show how on my YouTube channel, **[AI Automation Station](https://www.youtube.com/@ai-automation-station)**.

Every project below has a project page, and most have a **live demo you can try in your browser**.

[All projects](https://mikeholp87.github.io) · [YouTube](https://www.youtube.com/@ai-automation-station) · [Guides](https://www.ai-automation-station.com/guides.html) · [LinkedIn](https://www.linkedin.com/in/mikeholp) · [X](https://x.com/mikeholp) · [Sponsor](https://github.com/sponsors/mikeholp87)

## Open source desktop apps

| | |
|---|---|
| <a href="https://github.com/mikeholp87/Tasky"><img src="https://mikeholp87.github.io/Tasky/assets/overview-dark-720.webp" alt="Tasky, a Linux and Windows task manager and system monitor, showing CPU, memory, storage and network graphs" width="320"></a> | **[Tasky](https://github.com/mikeholp87/Tasky): Linux and Windows task manager and system monitor**<br>Live CPU, memory, disk and network graphs, process control, benchmarks and no telemetry. Works on KDE Plasma and GNOME. Built with Tauri, Rust and React.<br>[Project page](https://mikeholp87.github.io/Tasky/) · [Try the demo](https://mikeholp87.github.io/Tasky/demo/) |
| <a href="https://github.com/mikeholp87/Luma-Launcher"><img src="https://mikeholp87.github.io/Luma-Launcher/assets/palette-dark-680.webp" alt="Luma Launcher, a Linux application launcher, listing apps in a keyboard-driven search palette" width="320"></a> | **[Luma Launcher](https://github.com/mikeholp87/Luma-Launcher): keyboard-driven Linux app launcher**<br>Fuzzy app search, favorites, a calculator and web search keywords. Rust and GTK4.<br>[Project page](https://mikeholp87.github.io/Luma-Launcher/) · [Try the demo](https://mikeholp87.github.io/Luma-Launcher/demo/) |
| <a href="https://github.com/mikeholp87/update-forge"><img src="https://mikeholp87.github.io/update-forge/assets/dashboard-dark.png" alt="Update Forge, a software updater for Windows 11 and Linux, showing available updates" width="320"></a> | **[Update Forge](https://github.com/mikeholp87/update-forge): software updater for Windows 11 and Linux**<br>Finds outdated apps and updates them through WinGet, apt, Flatpak, Snap and npm. No telemetry, no accounts. C# and .NET.<br>[Project page](https://mikeholp87.github.io/update-forge/) · [Try the demo](https://mikeholp87.github.io/update-forge/demo/) |
| <a href="https://github.com/mikeholp87/aegis-vpn"><img src="https://mikeholp87.github.io/aegis-vpn/screenshot.webp" alt="Aegis VPN, an open source WireGuard client for Linux, showing a verified kill switch and DNS leak protection" width="320"></a> | **[Aegis VPN](https://github.com/mikeholp87/aegis-vpn): open source WireGuard client for Linux**<br>Bring your own server. Verified kill switch, DNS and IPv6 leak checks. Pre-alpha, written in Rust and Tauri.<br>[Project page](https://mikeholp87.github.io/aegis-vpn/) · [Try the demo](https://mikeholp87.github.io/aegis-vpn/demo/) |
| <a href="https://github.com/mikeholp87/Restic-Studio"><img src="https://mikeholp87.github.io/Restic-Studio/assets/backup-dark-640.webp" alt="Restic Studio, a Restic GUI for Linux backups, showing the Backup tab" width="320"></a> | **[Restic Studio](https://github.com/mikeholp87/Restic-Studio): Restic GUI for Linux backups**<br>Encrypted backups to local folders and external drives, snapshot browsing and safe restores without the command line. Early preview. Rust and GTK4.<br>[Project page](https://mikeholp87.github.io/Restic-Studio/) · [Try the demo](https://mikeholp87.github.io/Restic-Studio/demo/) |
| <a href="https://github.com/mikeholp87/strata-editor"><img src="https://mikeholp87.github.io/strata-editor/screenshot.png" alt="Strata Editor, a Markdown and code editor for Linux, showing Markdown source and a live preview" width="320"></a> | **[Strata Editor](https://github.com/mikeholp87/strata-editor): native Markdown and code editor**<br>Text, code, Markdown and formatted HTML with split views and live preview. Offline, no telemetry. C++20 and Qt 6.<br>[Project page](https://mikeholp87.github.io/strata-editor/) · [Try the demo](https://mikeholp87.github.io/strata-editor/demo/) |

More: [Disk Atlas](https://github.com/mikeholp87/disk-atlas) (Linux disk usage analyzer with sunburst and treemap views), [ExtentPilot](https://github.com/mikeholp87/defrag-hdd-linux) (Linux file extent and fragmentation analyzer), [NUC Control](https://github.com/mikeholp87/msi-control-linux) (Linux hardware and power monitor for MSI mini PCs) and [herdr-mods](https://github.com/mikeholp87/herdr-mods) (mods for the Herdr app).

## Install on Debian and Ubuntu

Tasky, Luma Launcher, Restic Studio and Strata Editor install from my signed apt repository, so
`apt install` and `apt upgrade` work as usual:

```bash
sudo install -d -m 0755 /etc/apt/keyrings
curl -fsSL https://mikeholp87.github.io/apt/apt.asc | sudo tee /etc/apt/keyrings/mikeholp87-apt.asc >/dev/null
echo "deb [signed-by=/etc/apt/keyrings/mikeholp87-apt.asc] https://mikeholp87.github.io/apt/ ./" | sudo tee /etc/apt/sources.list.d/mikeholp87-apt.list
sudo apt update
sudo apt install tasky
```

Details and the full package list: [mikeholp87.github.io/apt](https://mikeholp87.github.io/apt/).

## Skills and technologies

- **Languages:** Rust, C++20, TypeScript, JavaScript, C#, Shell. Earlier iOS apps in Objective-C and Swift (2013 to 2014).
- **Desktop frameworks:** Tauri 2, GTK4 and libadwaita, Qt 6, egui and wgpu, Avalonia and .NET, React and Vite.
- **Linux and systems:** KDE Plasma and GNOME, Wayland and X11, systemd, NetworkManager, WireGuard, Restic, FIEMAP, Debian packaging and signed apt repositories.
- **Delivery:** GitHub Actions CI and releases, GitHub Pages, Vercel, release automation and security hardening for packaged apps.
- **AI-assisted development:** building and shipping real apps with Claude Code, Codex and OpenCode, plus the AI Automation Station videos and guides that document the process.

## Build guides and videos

- [Claude Code Task Manager: scope, checks and packaging](https://www.ai-automation-station.com/guides/claude-code-task-manager.html) (Tasky)
- [UpdateForge: Windows and Linux package manager GUI](https://www.ai-automation-station.com/guides/updateforge-package-manager-windows-linux.html)
- [Aegis VPN with Claude Code: build and test the client](https://www.ai-automation-station.com/guides/aegis-vpn-claude-code.html)
- [Herdr desktop guide: setup, workspaces and limits](https://www.ai-automation-station.com/guides/herdr-desktop-app.html)
- [Tasky, Restic Studio and Luma Launcher: project demos](https://www.ai-automation-station.com/watch/V0PoYhOprBI)

## More from me

- **Written guides and videos:** [ai-automation-station.com](https://www.ai-automation-station.com)
- **Learning community:** [AI Income Lab](https://www.ai-automation-station.com/ai-income-lab.html) on Skool
- **Products I run:** [TubeAnalytics](https://www.tubeanalytics.net) (YouTube analytics) and [VisiScan](https://www.visiscan.app) (AI search visibility)

If a project is useful to you, a star on the repo helps other people find it, and you can support the work through [GitHub Sponsors](https://github.com/sponsors/mikeholp87).

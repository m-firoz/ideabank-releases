# Idea Bank

A local-first desktop app for capturing ideas and taking them from "a thought" to "built". Everything you write stays on your own computer — no account, no cloud, no tracking.

**Windows 10 / 11 (64-bit).**

## Download

1. Open the [**latest release**](https://github.com/m-firoz/ideabank-releases/releases/latest).
2. Under **Assets**, download the file ending in **`-setup.exe`**. (The other files are used by the app's built-in updater; you don't need them.)
3. Run it and follow the installer.

**Windows may say "Windows protected your PC".** That's SmartScreen reacting to a new app that isn't code-signed yet; it does not by itself mean the app is unsafe. Click **More info**, then **Run anyway**.

The installer downloads Microsoft's WebView2 runtime if your PC doesn't already have it (Windows 10/11 usually do), so the first install may need an internet connection.

## What it does

- **Dashboard** of all your ideas — one grid or grouped **By Status** — with **search** and **tag filtering**, and **undo** for a deleted idea.
- Each idea moves through Captured → Researching → Defined → Building → Completed, and can be put On Hold or Archived and resumed later.
- **About** — a rich-text write-up with an image gallery.
- **Brainstorm** — a free canvas of sticky notes.
- **Tasks**, **Pipeline / What's next**, **Links** and **Local Files** for each idea. Local Files keeps a *reference* to a file on your computer and takes you to it in Explorer; it never copies or changes the file.
- **Connections** — link two ideas with a note about why they relate.
- **Settings** — export and restore a full backup, and an optional switch for website icons on links.

## Your data and privacy

Your ideas are stored on your own disk under `%APPDATA%\com.ideabank.app` (paste that into the File Explorer address bar). Idea Bank never sends them anywhere. It makes only two kinds of network request:

- **Update check** — a few seconds after it starts, it asks this repository's releases page whether a newer version exists (GitHub can see your IP address and the app version, like any download). If one exists, a card offers **Install and restart**; nothing is installed without your click, and every update is cryptographically signed — the app refuses one that isn't.
- **Site icons — off by default.** If you turn on *Settings → Show site icons*, it asks DuckDuckGo's icon service for each saved link's icon, which tells them the website addresses you have saved. With it off, nothing is contacted for your links.

**Backups:** *Settings → Export backup…* saves everything — ideas, notes, links, tasks and images — into one file you choose the location of; *Restore from backup…* replaces everything with such a file after asking you to confirm. Keep backups somewhere other than the same drive.

## About this repository

This repository only hosts the downloads and holds no code. Idea Bank's source code is not published. If something doesn't work, please [open an issue](https://github.com/m-firoz/ideabank-releases/issues) and say what you did and what happened.

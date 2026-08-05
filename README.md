# Chrome Classic Menu Bar

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-blue)](#requirements)
[![Language](https://img.shields.io/badge/language-C%2B%2B-blue)](src/chrome-classic-menu-bar.wh.cpp)
[![Version](https://img.shields.io/badge/version-1.1.0-brightgreen)](CHANGELOG.md)
[![Windhawk Mod](https://img.shields.io/badge/Windhawk-mod-4b7bec)](https://windhawk.net/)

A Windhawk mod that adds a native Win32 **File, Edit, View, History, Bookmarks/Favorites, Tools, and Help** menu bar to **Google Chrome** and **Microsoft Edge**.

## Releases

See [CHANGELOG.md](CHANGELOG.md) for the complete list of releases and upgrade notes.

## Features

- Native Win32 menu bar integrated into browser windows.
- Supports **Google Chrome** and **Microsoft Edge** from a single codebase.
- Automatic runtime detection of Chrome or Edge.
- Browser-specific handling of internal pages (`chrome://` and `edge://`).
- File, Edit, View, History, Bookmarks/Favorites, Tools, and Help menus.
- Dark owner-drawn menu mode with a runtime toggle.
- Standard browser keyboard shortcuts and commands.
- Automatic attachment to existing browser windows.
- Automatic attachment to newly created browser windows.
- Automatic recovery if the browser recreates its native window.
- High compatibility with modern Chromium releases.
- Windows 10 and Windows 11 compatible.

## Supported Browsers

- Google Chrome (`chrome.exe`)
- Microsoft Edge (`msedge.exe`)

## Requirements

- Windows 10 or Windows 11.
- Windhawk.
- Google Chrome or Microsoft Edge.

## Install in Windhawk

1. Open Windhawk.
2. Select **Create a new mod**.
3. Copy the contents of `src/chrome-classic-menu-bar.wh.cpp`.
4. Paste the source into the Windhawk editor.
5. Click **Compile Mod**.
6. Enable the mod.
7. Restart Chrome or Edge if the menu bar does not appear immediately.

## Menu Commands

The mod provides familiar browser commands including:

- New Tab
- New Window / InPrivate Window
- Open File
- Save Page
- Print
- Undo / Redo
- Cut / Copy / Paste
- Reload
- Zoom
- Full Screen
- Page Source
- History
- Downloads
- Bookmarks / Favorites
- Extensions
- Settings
- Help
- About Browser

Most commands use the browser's native keyboard shortcuts. Browser-specific pages automatically open using the correct internal URL for Chrome or Edge.

## Dark Menu Mode

Select **View → Dark Menu Mode** to switch between the custom dark menu theme and the standard Windows menu colours.

The selected mode remains active while the mod is loaded.

## Source Layout

```text
src/chrome-classic-menu-bar.wh.cpp
    Main Windhawk source.

windhawk-submission/mods/
    Copy prepared for Windhawk submission.

.github/
    GitHub workflows and templates.

docs/
    Documentation.

screenshots/
    Project screenshots.
```

## Screenshots

Suggested screenshots:

- Chrome Dark Menu
- Chrome Light Menu
- Edge Dark Menu
- Edge Light Menu
- File Menu
- Tools Menu

## Known Limitations

- Future Chromium updates may require compatibility adjustments.
- Commands implemented through keyboard shortcuts depend on those shortcuts remaining unchanged.
- Dark Menu Mode is currently session-based and is not persisted between mod reloads.

## Contributing

Pull requests, bug reports, and feature suggestions are welcome.

Please read **CONTRIBUTING.md** before submitting changes.

## Security

Please see **SECURITY.md** for responsible vulnerability reporting.

## Author

Created by **Gokhan**

GitHub: https://github.com/GokhanGerkz

## License

Released under the **MIT License**.

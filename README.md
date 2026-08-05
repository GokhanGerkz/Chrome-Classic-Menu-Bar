# Chrome Classic Menu Bar

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-blue)](#requirements)
[![Language](https://img.shields.io/badge/language-C%2B%2B-blue)](src/chrome-classic-menu-bar.wh.cpp)
[![Windhawk Mod](https://img.shields.io/badge/Windhawk-mod-4b7bec)](https://windhawk.net/)

A Windhawk mod that adds a native Win32 **File, Edit, View, History, Bookmarks, Tools, and Help** menu bar to Google Chrome.

## Features

- Native menu bar attached to Chrome browser windows.
- File, Edit, View, History, Bookmarks, Tools, and Help menus.
- Dark owner-drawn menu mode with a runtime toggle.
- Common Chrome keyboard actions and internal Chrome pages.
- Automatic attachment to existing and newly created Chrome windows.
- Periodic recovery if Chrome recreates or replaces a browser window.
- DPI-aware menu sizing and font handling.
- Windows 10 and Windows 11 compatible design.

## Requirements

- Windows 10 or Windows 11.
- Google Chrome (`chrome.exe`).
- Windhawk.

## Install in Windhawk

1. Open Windhawk.
2. Select **Create a new mod**.
3. Copy the contents of [`src/chrome-classic-menu-bar.wh.cpp`](src/chrome-classic-menu-bar.wh.cpp).
4. Replace the editor contents with the copied source.
5. Select **Compile Mod**, then enable it.
6. Restart Chrome if the menu bar does not appear immediately.

## Menu commands

The mod exposes standard browser actions such as new tab, new window, open file, save, print, undo, redo, reload, zoom, full screen, history, bookmarks, downloads, extensions, settings, Chrome help, and About Chrome.

Some commands are implemented by sending Chrome's normal keyboard shortcuts. Internal pages such as bookmarks, extensions, settings, and About Chrome are opened in a new tab.

## Dark menu mode

Open **View → Dark Menu Mode** to switch between the custom dark menu and the normal system menu colours. The setting is active for the current loaded mod session.

## Source layout

```text
src/chrome-classic-menu-bar.wh.cpp       Main Windhawk mod source
windhawk-submission/mods/                Copy prepared for Windhawk pull request
.github/                                 GitHub templates and validation workflow
docs/                                    Installation and technical notes
screenshots/                             Place project screenshots here
```

## Screenshots

Add your screenshots to the `screenshots` directory and update this section before publishing images publicly.

Suggested files:

- `chrome-dark-menu.png`
- `chrome-light-menu.png`
- `file-menu.png`
- `tools-menu.png`

## Known limitations

- Chrome can change its native window implementation, which may require future compatibility updates.
- Commands based on synthetic keyboard input depend on Chrome retaining the corresponding shortcuts.
- The dark-mode choice is not currently persisted between mod reloads.
- The mod is designed specifically for `chrome.exe`; Chromium-based browsers with different executable names are not included.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## Security

See [SECURITY.md](SECURITY.md) for responsible reporting instructions.

## Author

Created by **Gokhan** — GitHub: **GokhanGerkz**.

## License

Released under the [MIT License](LICENSE).

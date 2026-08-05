# Chrome Classic Menu Bar v1.0.0

First stable public release of Chrome Classic Menu Bar.

## Highlights

- Native Win32 menu bar for Google Chrome.
- File, Edit, View, History, Bookmarks, Tools, and Help menus.
- Dark menu mode.
- Automatic attachment to current and newly created Chrome windows.
- Recovery when Chrome recreates its browser window.
- DPI-aware owner-drawn menus.
- Launchers for Chrome bookmarks, extensions, settings, downloads, and About Chrome.

## Installation

Install through Windhawk's mod editor using `src/chrome-classic-menu-bar.wh.cpp`, or install from the Windhawk repository after the mod is accepted there.

## Upgrade notes

This release changes the public version number from development version 0.6.0 to 1.0.0. The functional source is otherwise based on the supplied working implementation.

# Chrome Classic Menu Bar v1.1.0

Adds official Microsoft Edge support while preserving the existing Google Chrome experience.

## Highlights

- Official support for **Google Chrome** and **Microsoft Edge**.
- Automatic runtime detection of Chrome or Edge.
- Native Win32 **File, Edit, View, History, Bookmarks/Favorites, Tools, and Help** menu bar.
- Browser-specific handling of internal pages (`chrome://` and `edge://`).
- Edge-specific menu terminology, including **InPrivate**, **Favorites**, and **Microsoft Edge Help**.
- Dark menu mode.
- Automatic attachment to existing and newly created browser windows.
- Automatic recovery when the browser recreates its native window.
- Owner-drawn native menus.
- Launchers for Settings, Extensions, Downloads, History, Bookmarks/Favorites, and About pages.

## Installation

Install through Windhawk's mod editor using `src/chrome-classic-menu-bar.wh.cpp`, or install from the Windhawk repository once the mod update has been accepted.

## Upgrade Notes

This release expands the mod from **Google Chrome** to both **Google Chrome** and **Microsoft Edge** while maintaining a single shared codebase.

Existing Chrome functionality is preserved, and Edge-specific commands automatically use the appropriate internal pages and browser terminology.

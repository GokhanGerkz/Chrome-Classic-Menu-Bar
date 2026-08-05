# Technical Notes

The mod hooks `CreateWindowExW` to observe Chrome browser-frame creation and removes `WS_EX_NOREDIRECTIONBITMAP` for compatible native non-client rendering. It also hooks `SetWindowThemeAttribute` to prevent Chrome from disabling native non-client controls.

Chrome top-level windows are identified by the `Chrome_WidgetWin_` class prefix, a caption style, root-window status, and ownership by the current process.

Each attached Chrome window receives:

- A generated Win32 menu hierarchy.
- A cross-thread window subclass.
- Owner-draw and measure handling.
- Command dispatch for Chrome shortcuts and internal pages.

A watcher periodically enumerates windows to attach or restore the menu when Chrome recreates a frame. A message-only window manages custom global hotkeys while Chrome is active.

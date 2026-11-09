# Changelog

## Unreleased

<<<<<<< HEAD
- Fixed: files did not transfer with rclone 1.75 (Haul passed an option that version no longer has); any message rclone prints is now shown and logged instead of "stopped".
- Every error and crash now reaches the creator's dashboard (batched, anonymous: user name, e-mail and IP addresses removed); crash reports include the crashed thread from macOS's own report.
- Small windows: each pane fits its columns to its width, labels fold into icons, the transfer list stays under a third of the window — nothing overlaps.
- New: tiles view per pane, free space on a server in the pane's footer, an overall progress bar for transfers.
- The light icon is now the app's icon.
=======
## Haul 1.0.6 — 09-Nov-2026
>>>>>>> origin/main

- Fixed: "Restart to update" and quitting crashed on macOS 27 while closing the window; Haul now quits cleanly and the update installs and reopens.

## Haul 1.0.5 — 09-Nov-2026

- New app icon in the same style as the creator's other apps (dark tile, amber glow, amber crate, teal arrows).

## Haul 1.0.4 — 09-Nov-2026

- New: drag to select files — press beside a name and draw a box; ⌘ while dragging deselects rows already selected, clicking empty space clears.
- Fixed: copying onto a file of the same name now really replaces it (FTP servers report no usable date, so it used to be skipped); you can also choose Skip.

- Fixed: Haul closed by itself on macOS 27 a minute after opening (the window's file-drop handling confused the system's view scanning).
- The app icon shows at the top of the README on GitHub again.

## Haul 1.0.3 — 09-Nov-2026

## Haul 1.0.0 — 09-Nov-2026

## 1.0.0 — 2026-11-09

- First release: two panes (this Mac, servers and clouds side by side), 18 kinds of server through rclone, transfer queue with progress, drag and drop, sync (update, mirror, both ways) and compare, servers as disks in Finder without macFUSE, share links, quick look, Open in Terminal for SFTP, Haul Pro.

# Changelog

## Unreleased

## Haul 1.0.14 — 09-Nov-2026

- FTP much faster, like FileZilla: every connection uploads, checks no longer hold connections, no re-check after each upload.
## Haul 1.0.13 — 09-Nov-2026

- Finder disks: wait up to a minute for slow FTP logins, mount beside a disk macOS won't release, and say why when a mount fails.
- Fixed: single files failed with "can't limit to single files when using filters".
- Errors now reach the ipconfig dashboard (Crashes & errors): sent to /errors in batches under the size limit, retried when offline.
## Haul 1.0.12 — 09-Nov-2026

- Unfinished transfers resume by themselves after a quit, crash or update.
- About the author: call directly on +91 73972 85837 (WhatsApp is not checked).
- About › The creator: "Open to work" — full-stack roles, remote or in Chennai, ₹50,000 a month take-home (about ₹7–7.5 lakh CTC), with Email, WhatsApp and Résumé buttons.

## Haul 1.0.11 — 09-Nov-2026

- Disks in Finder come back by themselves when Haul opens again (after quitting or an update), and a disk left behind by a crash or a forced quit is cleared first, so it can be mounted again instead of failing.

## Haul 1.0.10 — 09-Nov-2026

- Even faster: several selected items now go across in ONE rclone run (one start-up and one login, every file in parallel) instead of one run each; a single file skips listing the destination folder; fast listing for S3, B2 and Drive.
- Settings › Transfers: pieces per big file (1–32) and connections per FTP/SFTP server (1–32), for servers that allow more — or fewer.

- Updates come from GitHub by default; the Cloudflare copy on ipconfig.co.network is the fallback when GitHub is slow or unreachable.

- Much faster transfers: 16 files at once by default (free up to 8, Pro up to 64), up to 16 items running together, big files split into 8 parallel streams, 32 checkers, a 64 MB read-ahead, and parallel connections for FTP (8), SFTP (64), S3, B2, Drive, OneDrive and Dropbox.
- Faster updates: the feed on ipconfig.co.network now points at Cloudflare copies of the download; a slow or failed download switches to the other copy (GitHub) by itself.

## Haul 1.0.9 — 09-Nov-2026

- Haul Pro as an auto-renewing Razorpay subscription: Subscribe (₹349 a month or ₹3,499 a year) starts it on your account; Pay once stays for a single month or year.

## Haul 1.0.8 — 09-Nov-2026

- Fixed: copying and moving did nothing — Haul put its log options after the file paths, so rclone printed its usage instead of transferring. The test stand-in now refuses that exactly as rclone does.

- Settings › Updates and reports: a Check for updates button with the version and when Haul last looked.
- Fixed: Download and install unpacks the update with tar (the release is a tar.gz); if anything fails, the window offers Try again and the DMG, and the failure reaches the creator's dashboard.
- Haul Pro: ₹349 a month, ₹3,499 a year.

## Haul 1.0.7 — 09-Nov-2026

- Fixed: the Activity and diagnostics window and every other window now fit the screen in short windows and scroll inside, instead of being cut off; long paths wrap.

- Fixed: files did not transfer with rclone 1.75 (Haul passed an option that version no longer has); any message rclone prints is now shown and logged instead of "stopped".
- Every error and crash now reaches the creator's dashboard (batched, anonymous: user name, e-mail and IP addresses removed); crash reports include the crashed thread from macOS's own report.
- Small windows: each pane fits its columns to its width, labels fold into icons, the transfer list stays under a third of the window — nothing overlaps.
- New: tiles view per pane, free space on a server in the pane's footer, an overall progress bar for transfers.
- The light icon is now the app's icon.

## Haul 1.0.6 — 09-Nov-2026

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

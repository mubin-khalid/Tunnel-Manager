# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Added
- Per-tunnel enable/disable toggle with active counter (`X / Y enabled`)
- Free plan guard: blocks enabling a 4th tunnel with a tooltip warning
- `tunnel-definitions.json` as the source of truth for tunnel definitions
- Auto-migration of existing `ngrok.yml` tunnels on first launch (all enabled by default)

### Changed
- `ngrok.yml` is now generated at start time from enabled tunnels only
- Dashboard empty state now reflects enabled tunnels, not total defined
- Start is blocked with an error message if no tunnels are enabled

### Fixed

### Removed

---

## [0.1.1] - 2025-01-01

### Added
- Initial public release
- Dashboard: start/stop ngrok and view active tunnel URLs
- Tunnels: add, edit, and delete tunnel definitions from the UI
- Settings: save ngrok authtoken and optionally auto-start on launch
- macOS DMG and Linux AppImage builds via GitHub Actions
- System tray icon with Show/Quit menu
- Auto-migration of legacy ngrok config locations on first launch
- Copy tunnel URL to clipboard from the Dashboard

---

[Unreleased]: https://github.com/mubin-khalid/tunnel-manager/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/mubin-khalid/tunnel-manager/releases/tag/v0.1.1
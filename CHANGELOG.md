# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]
### Added
- Lyric source order can now be customized by the user via command palette, with persistent global configuration.
- Periodic latency ping for each lyric source (LrcLib, Netease, QQMusic) to monitor API responsiveness.
- Status bar tooltip now displays average latency for each lyric source, with colored badges (🟢, 🟡, 🔴) for quick visual feedback.
- Webview panel displays the actual lyric source for the current song.
- Improved error handling and user feedback for network and permission issues.

### Changed
- Lyric source latency is now measured by scheduled ping, not by actual lyric fetch requests.
- Lyric source order is always stored in VSCode global settings, not workspace settings.
- Status bar text no longer displays latency badges; latency is only shown in the tooltip.
- All code comments are now in English for better maintainability.

### Fixed
- Fixed issues with command registration and activation events for custom commands.
- Fixed bugs where only the first lyric source latency was shown on first load.
- Improved robustness of lyric fetching and caching logic.

---

Older changes are not tracked in this changelog. 
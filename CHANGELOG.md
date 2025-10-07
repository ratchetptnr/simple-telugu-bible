# Changelog

All notable changes to Simple Telugu Bible will be documented here.

## [v0.1.0] - 2025-10-03

### Added
- Complete Telugu Bible text (USFM format)
- AI voice navigation with Gemini integration
- Adaptive typography (14-28pt font size)
- Adjustable line spacing (4-16pt)
- Auto-save reading position
- Cross-platform: iOS (SwiftUI) and Android (Jetpack Compose)
- Dark mode support
- High contrast verse numbers
- Large touch targets for elderly users
- Conversational AI handling Telugu/English/mixed input

### Technical
- iOS: SwiftUI + AppStorage for persistence
- Android: Jetpack Compose + DataStore
- Gemini 2.5 Flash Lite for voice processing
- USFM Bible text format
- Instant first chapter load, background loading for rest
- Verse-level highlighting with visual feedback

---

## How to Update This File

When you make changes to the app:

1. Add a new version header with date
2. Organize changes under: Added, Changed, Fixed, Removed
3. Keep entries concise and user-focused
4. Commit and push to update the website

Example format:
```markdown
## [v0.2.0] - 2025-10-07

### Added
- New feature description

### Fixed
- Bug fix description
```

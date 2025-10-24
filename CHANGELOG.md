# Changelog

All notable changes to Simple Telugu Bible will be documented here.

## [v0.0.7] - 2025-10-24

### Released
- **AI Chat Assistant now in production!** 🎉
- Full version (0.0.3-full) available on Play Store with AI features

### Added
- AI Chat Assistant powered by Gemini
- Multi-turn conversations about Bible verses, theology, and scripture
- Persistent chat history (all your conversations saved locally)
- Markdown-formatted AI responses
- Chat list with multi-select delete
- Message timestamps
- Keyboard shortcuts (press Enter to send)
- Smart auto-scrolling

### Technical
- APK size: 5.2 MB (signed, minified release build)
- R8/ProGuard optimization enabled
- Production keystore signing
- Version code: 3

---

## [v0.0.6] - 2025-10-20

### Fixed
- Fixed all padding and spacing issues throughout the app
- AI Chat input bar now has proper height without excessive padding
- Removed visible color seams between app bars and content in Settings, Book Selector, and About screens
- All screens now have seamless, professional appearance matching Android system apps

### Changed
- Major architecture refactor following Google's "Now in Android" best practices
- Migrated from 5+ nested Scaffolds to single top-level Scaffold pattern
- Improved visual consistency across all secondary screens

### Technical
- **Breaking architectural change**: Removed all nested Scaffolds (NEVER nest Scaffolds!)
- Implemented single Scaffold pattern with `contentWindowInsets = WindowInsets(0, 0, 0, 0)`
- Moved all TopAppBars from `Scaffold.topBar` parameter to content area
- Added proper `.consumeWindowInsets()` for correct inset consumption
- Applied `surfaceContainer` background color to secondary destinations for Material 3 compliance
- Each system inset now applied exactly once in component hierarchy
- Performance improvements from fewer unnecessary compositions

---

## [v0.0.5] - 2025-10-19

### Changed
- Renamed "AI Assistant" to "AI Chat" for better clarity
- Implemented standard Android multi-select pattern for chat list
  - Long-press any chat to enter selection mode
  - Select multiple chats and delete them at once
  - Visual feedback with checkboxes

### Fixed
- Fixed subtle layout jerk when entering selection mode
- Improved accessibility with proper touch target sizing

### Technical
- Migrated to Material 3 ListItem component for better standards compliance
- Follows Material Design patterns used in Gmail, Google Photos, and Files apps

---

## [v0.0.4] - 2025-10-17

### Changed
- Major Material 3 Expressive upgrade
- Bible screen now features collapsing app bar that expands/collapses as you scroll
- Smoother navigation animations between Bible and AI Chat tabs (crossfade instead of slide)
- Updated all screens to match Material 3 design specifications

### Fixed
- Fixed status bar color to match app bar (edge-to-edge display)
- Fixed app bar height issues across all screens
- Improved color consistency throughout the app

### Technical
- Updated to Material 3 Expressive (Compose Material 3 1.4.0-alpha06)
- Implemented LargeFlexibleTopAppBar for dynamic reading experience
- Proper edge-to-edge implementation with window insets

---

## [v0.0.3] - 2025-10-13

### Changed
- Updated settings icon from text icon (Tt) to standard settings cog icon
- Improved UX based on closed testing feedback

### Status
- **Android**: Now in closed testing on Google Play Store
- **iOS**: Coming soon

---

## [v0.0.2] - 2025-10-10

### Changed
- Play Store release preparation (Basic Version)
- APK size optimized: 16MB → 4.5MB (72% reduction)
- Removed all permissions for privacy-first approach
- Clean version numbering

### Fixed
- Chapter changes now reset to verse 1
- App saves and restores exact verse position on restart
- Book changes reset to chapter 1, verse 1

### Technical
- R8/ProGuard minification and resource shrinking enabled
- Created upload keystore for Google Play App Signing
- Privacy policy added

---

## [v0.0.1] - 2025-10-03

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

# Changelog

All notable changes to Movie Night Spinner are documented in this file.

## 09-AUG-2026

### Added

- Winner History edit page (`edit.html`) for managing saved winners
- Inline edit and remove for winner name and date
- Clear all winners (with confirmation)
- Undo / redo with toolbar buttons and keyboard shortcuts
- Sticky toolbar and status message while scrolling long lists
- Export winner history as `movie-night-winners.json`
- Upload JSON to replace history (after confirmation)
- Link from `wheel.html` to **Edit History**

### Security

- JSON upload validation (array of `{ name, date }` string fields only)
- Extra fields stripped on import
- Upload limits: 1MB file size, 5,000 winners max, 200 characters per field

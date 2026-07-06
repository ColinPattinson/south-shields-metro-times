# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-05-14 - [WCAG AA Compliance for Departure Status]
**Learning:** The previous background colors (#27ae60 and #3498db) did not meet WCAG AA contrast requirements when used with white text. Green #1b7a43 and Blue #206694 provide a 4.5:1 ratio or higher.
**Action:** Use #1b7a43 for 'Live/Good' states and #206694 for 'Scheduled/Info' states to ensure readability and accessibility.

## 2025-05-14 - [Screen Reader Context for Visual Indicators]
**Learning:** Visual-only indicators (like status dots or background colors) are inaccessible to screen readers.
**Action:** Use a `.sr-only` class to provide visually hidden textual context (e.g., "Live prediction:") alongside visual-only indicators.

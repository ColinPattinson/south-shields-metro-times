## 2025-05-14 - Screen Reader Context Pattern
**Learning:** Color-coded status indicators (like live vs scheduled) are invisible to screen readers and color-blind users. Using a visually hidden (.sr-only) label that updates alongside the visual state provides necessary context without cluttering the UI.
**Action:** Always pair visual-only state changes (background colors, icons) with a visually hidden text description for accessibility.

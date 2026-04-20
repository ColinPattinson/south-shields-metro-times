## 2026-04-20 - [Accessible Color Contrast & Screen Reader Context]
**Learning:** Standard status colors like #27ae60 (green) and #3498db (blue) fail WCAG AA contrast requirements when paired with white text on typical prediction bars; accessible alternatives like #1b5e20 and #1565c0 should be used instead. Also, using `.sr-only` to provide context for color-coded states (e.g., Live vs Scheduled) is essential for screen reader users.
**Action:** Always check color contrast for status indicators and provide a textual equivalent for information conveyed through color.

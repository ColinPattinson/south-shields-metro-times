## 2026-04-18 - [Accessible Contrast & Screen Reader Context]
**Learning:** Standard transit status colors (like #27ae60 for live/good and #3498db for static/info) can fail WCAG contrast checks against white text. Furthermore, using color alone to distinguish data sources (live vs. scheduled) is an accessibility failure (WCAG 1.4.1).
**Action:** Use darker, accessible alternatives like #1b5e20 and #1565c0, and always pair visual state changes with visually hidden text (`.sr-only`) to provide context for screen reader users.

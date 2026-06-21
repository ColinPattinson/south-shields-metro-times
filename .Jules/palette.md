## 2026-06-21 - Screen Reader Context Pattern
**Learning:** Color-coded status indicators (like green for live, blue for scheduled) are invisible to screen reader users and can be confusing for color-blind users if not supplemented with text. Using a visually hidden (.sr-only) label that updates its text alongside the visual change ensures all users receive the same state information.
**Action:** Always pair visual-only state indicators with a .sr-only element that describes the state, and use aria-live to announce changes if they happen dynamically.

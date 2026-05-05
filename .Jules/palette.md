## 2026-05-05 - Screen Reader Context Pattern for Color-Coded States
**Learning:** Visual-only state changes (like background color switching between live and scheduled) are invisible to screen reader users. Using a visually hidden element that updates its text alongside the color change ensures all users receive the same information.
**Action:** Always implement a `.sr-only` context label when using color to convey status or state transitions.

## 2026-05-05 - Color Contrast in Status Indicators
**Learning:** The application's use of #27ae60 (Green) and #3498db (Blue) for status backgrounds with white text fails WCAG AA contrast requirements (4.5:1).
**Action:** Audit and improve color palettes to ensure text remains readable for all users, especially in high-information density transit apps.

## 2026-05-20 - Screen Reader Context Pattern
**Learning:** For single-page apps that communicate state via background colors (e.g., Live vs. Scheduled), visual-only cues are inaccessible to screen reader users and those with color blindness. Using a visually hidden element (`.sr-only`) that updates its text content alongside visual changes ensures all users receive the same state information.
**Action:** Always pair visual state indicators with an accessible text label using the `.sr-only` pattern and use `aria-live` on the container to announce updates.

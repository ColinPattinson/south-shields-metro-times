## 2026-04-27 - Screen Reader Context Pattern
**Learning:** Conveying status through color alone (e.g., green for live, blue for scheduled) is inaccessible to screen reader and color-blind users. Using a visually hidden `sr-only` element that updates its text alongside the color change provides the necessary context without altering the visual design.
**Action:** Always pair visual-only status indicators with descriptive `sr-only` text or ARIA attributes that programmatically explain the current state.

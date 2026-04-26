## 2025-05-15 - Screen Reader Context Pattern
**Learning:** Purely color-coded states (like Green for Live vs Blue for Scheduled) are inaccessible to screen reader users and those with color vision deficiency. Using a visually hidden (`.sr-only`) span that updates its text content alongside the visual change ensures all users receive the same state information.
**Action:** Always pair visual-only state changes (color, icons, background) with an `.sr-only` description that explicitly states the current mode or status.

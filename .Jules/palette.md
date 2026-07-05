## 2026-07-05 - Screen Reader Context Pattern
**Learning:** For status indicators that rely on color (e.g., Green for Live, Blue for Scheduled), visual-only changes are inaccessible to screen reader users. Combining a visually hidden (`.sr-only`) label with `aria-live="polite"` on the parent container ensures the state change is announced clearly.
**Action:** Always pair color-coded status changes with a visually hidden text label and consider `aria-live` for dynamic updates.

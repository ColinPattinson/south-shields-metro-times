## 2025-05-14 - Screen Reader Context Pattern
**Learning:** For status indicators that rely on color (e.g., green for live, blue for scheduled), visual-only cues are insufficient for accessibility. Using a visually hidden element (`.sr-only`) that updates its text alongside the visual change ensures screen reader users receive the same state information.
**Action:** Always pair color-based status changes with a visually hidden text label and consider using `aria-live` on the parent container to announce updates.

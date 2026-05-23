## 2025-05-23 - Screen Reader Context Pattern
**Learning:** Color-coded states (like Green for Live and Blue for Scheduled) are inaccessible to screen reader and color-blind users without accompanying text. Using a visually hidden `.sr-only` span that updates its text alongside visual changes ensures that all users receive the same state information.
**Action:** Always pair visual-only state indicators with an `.sr-only` element that provides a text description of the current state. Use `aria-live="polite"` on the parent container to ensure these updates are announced.

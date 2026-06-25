## 2024-06-25 - Screen Reader Context Pattern
**Learning:** When using color-coded states (e.g., Green for Live, Blue for Scheduled), screen reader users lose this context. Applying `aria-live="polite"` to a container and updating a visually hidden `.sr-only` label alongside the visual change ensures all users receive the same state information.
**Action:** Always pair visual state indicators with accessible text descriptions or ARIA labels that update dynamically.

## 2026-04-28 - The Screen Reader Context Pattern
**Learning:** Color-coded status indicators (like green for live vs blue for scheduled) are inaccessible to color-blind and screen-reader users if color is the only indicator.
**Action:** Always pair visual state changes with a visually hidden (`.sr-only`) element that provides the same information in text, and use `aria-live` on the parent container to ensure the update is announced.

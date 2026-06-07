
## 2024-06-07 - Screen Reader Context Pattern for Color-Coded Status
**Learning:** When using color (like Green for 'Live' and Blue for 'Scheduled') to communicate application state, screen reader users miss this context unless it's explicitly provided in text. Using a visually hidden (.sr-only) label within an aria-live container allows for immediate and accessible state announcements without altering the visual design.
**Action:** Always pair visual state indicators (colors, icons) with a .sr-only text equivalent and consider aria-live="polite" for dynamic updates.

## 2024-06-07 - Addressing the Time 'Dead Zone' in Transit UIs
**Learning:** A strictly greater-than check (m > currentMinute) for departure times creates a 60-second 'dead zone' where a train departing *now* is hidden from the UI. An inclusive check (m >= currentMinute) combined with a "Due now" label provides much better user clarity for immediate departures.
**Action:** Use inclusive boundaries for time-based filtering and provide specific "Due now" feedback for zero-minute countdowns.

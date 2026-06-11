## 2026-06-11 - Screen Reader Context Pattern
**Learning:** In static apps using background colors to indicate state (e.g., Live vs. Scheduled), screen reader users lose critical information.
**Action:** Use a `.sr-only` class to provide visually hidden text that updates alongside the visual state, and wrap visual-only elements in `aria-hidden="true"`.

## 2026-06-11 - The Transit "Dead Zone"
**Learning:** Filtering scheduled departures with `m > currentMinute` creates a 60-second window where a train departing "now" is hidden from the user.
**Action:** Use `m >= currentMinute` and map 0-minute differences to "Due now" for better clarity and reliability.

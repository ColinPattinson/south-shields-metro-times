## 2026-05-04 - Screen Reader Context Pattern for State-based Styles
**Learning:** When using background colors (e.g., green/blue) to indicate state (Live/Scheduled), screen reader users miss this info. Adding a visually hidden `.sr-only` span that updates alongside the color ensures parity.
**Action:** Always pair visual color changes for state with a `.sr-only` label or ARIA attribute.

## 2026-05-04 - Transit Countdown "Due now" Clarity
**Learning:** Displaying "0 mins" for immediate departures is technically correct but less intuitive than "Due now".
**Action:** Implement conditional logic to display "Due now" when the countdown reaches zero.

## 2025-05-14 - Screen Reader Context for State Transitions
**Learning:** When using background colors to indicate state (e.g., green for 'Live' vs blue for 'Scheduled'), screen reader users lose this context. Using a visually hidden element (.sr-only) that updates its text alongside the visual change ensures parity.
**Action:** Always pair visual-only state indicators with a .sr-only label or ARIA attribute.

## 2025-05-14 - Transit Countdown "Due Now" and Inclusive Filtering
**Learning:** Users find "0 mins" confusing for imminent departures; "Due now" is more intuitive. Also, filtering schedules with `>` instead of `>=` creates a 60-second window where a train at the current minute is hidden.
**Action:** Use inclusive filtering for time-based displays and map 0-minute countdowns to "Due now".

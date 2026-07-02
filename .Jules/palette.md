## 2025-05-14 - Inclusive Time Filtering for Transit UX
**Learning:** In transit applications, filtering schedules for times strictly greater than the current minute creates a 60-second "dead zone" where upcoming departures are hidden but not yet marked as 'Due now'.
**Action:** Use inclusive checks (>=) for the current minute and map 0-minute differences to a "Due now" state to provide continuous and accurate feedback.

## 2025-05-14 - Screen Reader Context Pattern
**Learning:** Visual-only indicators (like status dots or background colors) lack semantic meaning for screen readers. Using a visually hidden (.sr-only) label that updates alongside these visual changes ensures assistive technology users receive the same state information.
**Action:** Always accompany visual state indicators with an `.sr-only` element describing the state, and use `aria-live` on containers where these states update dynamically.

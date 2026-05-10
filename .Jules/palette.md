## 2026-05-10 - Screen Reader Context Pattern
**Learning:** For dynamic UI components that use color to communicate state (e.g., Live vs Scheduled departures), visual users get immediate context while screen reader users may only hear the updated time. Using a visually hidden (.sr-only) label that updates its text content alongside the visual change ensures parity in information delivery.
**Action:** Always pair visual state indicators (like background colors or icons) with an `.sr-only` element that explicitly states the current status, and wrap the container in `aria-live="polite"` for automatic announcement.

## 2026-05-10 - Midnight Wrap-around Logic for Transit Apps
**Learning:** Transit schedules often operate across a 24-hour boundary. Simple subtraction for countdowns (Next - Now) fails after midnight or when looking ahead to the next morning.
**Action:** Use modulo 24 arithmetic for hour selection and always add 1440 minutes (24h) to countdown differences if the result is negative to correctly handle the day transition.

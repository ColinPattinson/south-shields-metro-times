## 2026-06-06 - Screen Reader Context Pattern
**Learning:** Color-coded status (like Live vs Scheduled) is invisible to screen readers and color-blind users if it's the only indicator.
**Action:** Use a visually hidden span (`.sr-only`) that updates its text alongside visual changes to ensure all users receive the same state information.

## 2026-06-06 - Schedule "Dead Zone" Prevention
**Learning:** Using an exclusive check (`m > currentMinute`) for departures creates a 60-second "dead zone" where a train departing right now is hidden, which can be confusing for users already at the platform.
**Action:** Use an inclusive check (`m >= currentMinute`) and display "Due now" for 0-minute wait times to provide immediate, actionable information.

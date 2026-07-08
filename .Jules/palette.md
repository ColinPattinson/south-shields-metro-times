## 2024-05-20 - [Aria-live and Visually Hidden Labels]
**Learning:** For a simple status dashboard, aria-live="polite" on a parent container effectively communicates updates. Visually hidden labels (status-label, indicator-text) provide necessary context for dynamic values (like times) that might be ambiguous to screen readers.
**Action:** Always wrap dynamic status values with descriptive visually-hidden labels and use aria-live for real-time updates.

## 2024-05-20 - [Due Now Logic and Inclusive Filtering]
**Learning:** Users prefer "Due now" over "0 mins" for immediate feedback. Inclusive filtering (>= currentMinute) ensures that departures occurring within the current minute are not prematurely hidden, preventing a 60-second "dead zone".
**Action:** Use inclusive checks for time-based filtering and implement intuitive "Due now" states for immediate events.

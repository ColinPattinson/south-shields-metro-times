## 2025-04-05 - Semantic Lists and Manual Refresh Logic
**Learning:** For time-sensitive public transit data, a semantic `<ul>` is significantly more useful for screen reader users than `<br>`-separated strings as it provides an immediate count of upcoming departures. Additionally, manual refresh buttons must use a `try...finally` pattern in JS to ensure the UI is never left in a permanently disabled "loading" state if a network request fails.
**Action:** Always prefer semantic list structures for data lists and use `try...finally` for all manual trigger loading states.

## 2025-04-05 - Immediate Departure Filtering
**Learning:** Users checking a departure board often expect to see trains that are departing in the current minute (0 mins wait). Filtering for `m > currentMinute` can cause confusion when a train is about to leave.
**Action:** Use inclusive logic (`m >= currentMinute`) and a "Due now" label for a better "just-in-time" user experience.

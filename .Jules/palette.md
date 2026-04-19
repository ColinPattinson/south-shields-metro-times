## 2026-04-19 - Accessible Context for Color-Coded State
**Learning:** Using color alone (e.g., green for live, blue for static) fails WCAG success criterion 1.4.1. Screen reader users miss the source of data if it's only communicated visually.
**Action:** Use the Screen Reader Context Pattern: pair visual color changes with a visually hidden element (`.sr-only`) that explicitly describes the state (e.g., "Live data" vs "Scheduled time").

## 2026-04-19 - Reliable Time-Dependent UI Verification
**Learning:** Testing "Due now" or countdown logic in static HTML apps requires precisely controlling the system time within the browser context.
**Action:** Inject a robust `window.Date` mock using Playwright's `page.add_init_script` that overrides `Date.now()` and the `Date` constructor to ensure consistent test results regardless of when the test runner executes.

## 2025-05-14 - Micro-UX improvements for countdowns and refresh states
**Learning:** Users find "Due now" more intuitive than "0 mins" for imminent departures. Consistent pluralization (1 min vs 2 mins) and visual feedback on manual refresh actions (loading states) significantly improve the perceived quality of the interface. Accessibility should be baked in using aria-live for dynamic updates and sr-only labels for color-coded status indicators.
**Action:** Always check for singular/plural logic in countdowns and ensure interactive elements provide immediate state feedback.

# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-05-14 - Initial Assessment
**Learning:** The application uses color-coded backgrounds (green for live, blue for static) to communicate state, which is not accessible to screen readers or color-blind users without additional context. The fallback to static times can also lead to a "dead zone" where departures in the current minute are hidden due to exclusive filtering.
**Action:** Use `.sr-only` labels to communicate state textually, improve color contrast for WCAG AA compliance, and use inclusive filtering for time-based logic.

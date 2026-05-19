# Palette's Journal

This journal contains critical UX and accessibility learnings for the South Shields Metro Times project.

## 2026-05-19 - Screen Reader Context for Dynamic Content
**Learning:** Visual-only indicators like background color changes (green for live, blue for scheduled) are invisible to screen reader users. Simply announcing the time isn't enough; the *context* of that time must also be communicated.
**Action:** Use the 'Screen Reader Context Pattern': a visually hidden span (`.sr-only`) inside an `aria-live` region that updates its text (e.g., "Live departure:") alongside visual changes to ensure all users receive the same state information.

## 2026-05-19 - Humanizing Countdown States
**Learning:** "0 mins" is technically correct but feels robotic and slightly ambiguous. Users prefer immediate, actionable language when a service is imminent.
**Action:** Implement a "Due now" state for 0-minute countdowns and ensure correct pluralization for other values to make the interface feel more polished and intuitive.

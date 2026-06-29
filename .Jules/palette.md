## 2025-05-14 - [Semantic Lists & Real-time States]
**Learning:** Using inclusive minute filtering (>=) for departure boards prevents a 60-second 'dead zone' where upcoming trains are hidden. Combining this with "Due now" text provides immediate, intuitive feedback that matches user expectations for live transport displays.

**Action:** Always check if time-based filters should be inclusive of the current minute to avoid missing immediate events.

## 2025-05-14 - [Screen Reader Context Pattern]
**Learning:** Visual-only indicators (like background color changes for 'Live' vs 'Scheduled' states) are inaccessible to screen reader users unless accompanied by text. The 'Screen Reader Context Pattern' (using .sr-only utility to provide descriptive labels) bridges this gap without cluttering the visual UI.

**Action:** Pair every significant visual state change with a corresponding visually hidden text update for assistive technology.

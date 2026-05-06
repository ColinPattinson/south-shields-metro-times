## 2023-10-27 - Screen Reader Context Pattern
**Learning:** Using color-only cues (like green for live, blue for scheduled) fails accessibility for color-blind and screen-reader users. A visually hidden span (.sr-only) that updates its text alongside visual state changes provides the necessary context for assistive technology without cluttering the UI.
**Action:** Always pair visual state changes (color, icons) with a visually hidden text description for screen readers.

## 2023-10-27 - Robust Relative Time
**Learning:** Relative time calculations (like "mins until") often fail at the midnight boundary, resulting in negative values. Simple modulo or conditional wrap-around (adding 1440 mins) ensures consistent behavior for late-night transit services.
**Action:** Implement midnight wrap-around logic for any time-difference calculations in transit apps.

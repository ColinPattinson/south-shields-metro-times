## 2025-05-14 - Enhancing Clarity for Dynamic Data Sources
**Learning:** Using color alone (e.g., green for live, blue for static) to indicate data freshness violates WCAG 1.4.1. Screen reader users need explicit text descriptions for these states. Additionally, departure countdowns should be inclusive of the current minute to avoid "missing" immediate trains.
**Action:** Always provide a visually hidden (`.sr-only`) label when status is communicated via color, and ensure time-based filters use inclusive boundaries (e.g., `>=`).

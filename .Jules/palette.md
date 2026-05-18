## 2025-05-14 - Screen Reader Context Pattern
**Learning:** Purely visual indicators (like background color changes or status dots) are invisible to screen reader users. Using a visually hidden span (`.sr-only`) that updates its text alongside visual changes ensures assistive technology users receive the same state information (e.g., "Live" vs "Scheduled").
**Action:** Always pair visual-only state changes (colors, icons) with `.sr-only` descriptive text or ARIA attributes.

## 2025-05-14 - Accessible Color Contrast for Status Indicators
**Learning:** Standard brand colors (like light blue #3498db or light green #27ae60) often fail WCAG AA contrast ratios (4.5:1) when paired with white text.
**Action:** Use darker variations (e.g., #206694 for blue, #1b7a43 for green) to ensure readability for users with visual impairments while maintaining the "color meaning" of the status.

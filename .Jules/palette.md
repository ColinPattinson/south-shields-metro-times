## 2024-07-07 - Accessibility and Contrast Improvement
**Learning:** The original brand colors (#3498db and #27ae60) did not meet WCAG AA contrast requirements when used as backgrounds for white text. Additionally, using color alone to indicate "Live" vs "Scheduled" states is inaccessible to screen reader users.
**Action:** Use WCAG-compliant colors (#206694 for Blue, #1b7a43 for Green) and implement visually hidden labels (.sr-only) with aria-live regions to communicate state changes to all users.

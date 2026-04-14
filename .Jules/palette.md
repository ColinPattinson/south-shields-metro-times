## 2026-04-14 - Accessible Contrast for Status Colors
**Learning:** Standard UI colors like #3498db (blue) and #27ae60 (green) often fail WCAG AA contrast requirements (4.5:1) when paired with white text on light backgrounds or used as border/text colors. Accessible alternatives like #1565c0 and #1b5e20 provide better readability while maintaining the same color intent.
**Action:** Always verify contrast ratios for status indicators and prediction bars, especially when they contain critical information like departure times.

## 2026-04-14 - Semantic Lists for Departure Times
**Learning:** Using string joining with `<br>` for lists of times (like departures) is a "flat" structure that prevents screen readers from announcing the total number of items or allowing users to jump between them easily.
**Action:** Use semantic `<ul>` and `<li>` elements for any list of discrete data points, even if they are styled to look like simple text blocks.

## 2026-04-13 - [Semantic Lists & Color Contrast]
**Learning:** Standard status colors (like #3498db and #27ae60) often fail WCAG AA contrast requirements on white backgrounds or with white text. Semantic `<ul>` lists are essential for screen readers to provide context (e.g., list item counts), whereas `<br>` separation provides no structural information.
**Action:** Always prefer semantic list elements over manual line breaks for lists of data. Use accessible color variants (#1565c0 for blue, #1b5e20 for green) for status indicators and high-contrast UI elements.

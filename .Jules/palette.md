## 2025-05-15 - Screen Reader Context Pattern
**Learning:** For status indicators that rely on visual-only cues (like background color or colored dots), using a sibling `.sr-only` span that updates its text content alongside the visual state ensures that assistive technology users receive the same information as sighted users without visual clutter.
**Action:** Always pair visual status indicators (e.g., #statusIndicator) with an adjacent `.sr-only` element (e.g., #indicator-text) and update both simultaneously in the UI logic.

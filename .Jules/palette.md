## 2026-04-11 - Accessibility and Clarity in Departure Information
**Learning:** Purely visual cues (like background color changes for live data) are inaccessible to screen reader users. Using a visually hidden `.sr-only` span provides necessary context without cluttering the UI. Semantic lists (`<ul>`/`<li>`) are superior to `<br>`-separated strings for assistive technology as they provide a count of items.
**Action:** Always pair visual state changes with screen-reader accessible text and use semantic list structures for collections of data like timestamps.

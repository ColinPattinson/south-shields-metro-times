## 2025-05-11 - Screen Reader Context Pattern for Live States

**Learning:** The application previously relied solely on background color (#27ae60 for Live, #3498db for Scheduled) to communicate data freshness. This violates WCAG 1.4.1 (Use of Color) and is inaccessible to screen reader users. By using a visually hidden `.sr-only` span that updates its text (e.g., "(Live)" or "(Scheduled)") alongside the visual color change, we provide the same context to all users without cluttering the visual UI.

**Action:** Always pair color-coded status changes with a visually hidden text label and `aria-live` regions to ensure state changes are perceivable and announced by assistive technologies.

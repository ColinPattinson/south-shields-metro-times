## 2025-05-14 - Screen Reader Context Pattern for Color-Coded States
**Learning:** Visual-only indicators (like background color changes from blue to green) are inaccessible to screen reader users and those with color blindness. Implementing an `.sr-only` span that updates its text (e.g., "(Live)" vs "(Scheduled)") alongside the visual change ensures state parity across all users.
**Action:** Always pair visual state changes (color, icons) with visually hidden text or ARIA attributes that describe the new state.

## 2025-05-14 - Contrast Ratios in Status Indicators
**Learning:** The application's default status colors (#27ae60 green and #3498db blue) with white text yield contrast ratios of 2.9:1 and 3.17:1, failing the WCAG AA 4.5:1 requirement for normal text.
**Action:** In future updates, propose higher-contrast color pairs or use dark text on light backgrounds for status badges to meet accessibility standards.

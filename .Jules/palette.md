## 2026-06-13 - Screen Reader Context Pattern
**Learning:** Purely visual state indicators (like background color changes for 'Live' vs 'Scheduled') are invisible to screen readers. Using an `aria-live` region combined with a visually hidden label (`.sr-only`) ensures that assistive technology users receive immediate and clear context for status updates.
**Action:** Always pair visual state changes with a corresponding `.sr-only` text update inside an `aria-live` container to provide equivalent information to all users.

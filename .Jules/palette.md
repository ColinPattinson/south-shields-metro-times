## 2026-04-02 - [Initial Accessibility and UX Review]
**Learning:** The application lacks `aria-live` regions for dynamic content, leading to screen reader users missing live updates. Additionally, simple minute counts (e.g., "1 mins") were discovered, highlighting the need for conditional pluralization.
**Action:** Implement `aria-live="polite"` on all dynamic time displays and use conditional logic for unit pluralization in future components.

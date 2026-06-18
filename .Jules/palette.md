## 2025-01-24 - Accessible Status Indicators and Inclusive Time Logic
**Learning:** For real-time departure boards, using exclusive minute checks (m > currentMinute) creates a 60-second "dead zone" where active departures disappear. Additionally, color-coded status indicators must be accompanied by visually hidden text and WCAG AA compliant colors (#1b7a43 for green, #206694 for blue) to ensure accessibility.
**Action:** Always use inclusive checks (m >= currentMinute) for "Due now" states and pair color changes with `.sr-only` text updates and `aria-live` regions.

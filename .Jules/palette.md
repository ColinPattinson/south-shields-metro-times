## 2024-05-15 - [Accessible State Communication]
**Learning:** Purely visual state indicators (like background color changes for 'Live' vs 'Scheduled') are inaccessible to screen reader users and those with color blindness.
**Action:** Use a visually hidden span with `.sr-only` inside an `aria-live` region to announce state changes textually, and ensure color changes use accessible contrast ratios (e.g., #1e8449 for green, #2980b9 for blue).

## 2024-05-15 - [Inclusive Time Filtering]
**Learning:** Using exclusive filtering (`m > currentMinute`) for upcoming events can cause a "jump" where an event occurring *now* disappears from the list before it's actually past.
**Action:** Use inclusive filtering (`m >= currentMinute`) and map 0-minute differences to a "Due now" label for better user clarity.

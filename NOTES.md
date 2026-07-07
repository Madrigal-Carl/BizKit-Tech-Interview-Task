### 1. The double-booking bug

The dates_overlap function only checked if a new booking's start date was within an existing booking. I updated the condition to detect all overlapping date ranges.

Existing: 10/01/2026 - 15/01/2026, New: 05/01/2026 - 13/01/2026 — the original code wrongly allowed this booking, while the updated condition correctly blocks it by checking both date ranges for overlap.

I used ChatGPT to review the dates_overlap logic. I verified the fix by reading the condition and manually testing different booking dates.

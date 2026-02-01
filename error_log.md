## Error Log

Absolutely — we can prepare a **Game Error Log** based on the session so far. This is useful for auditing, clarifying past moves, and ensuring consistency in future turns. I’ve gone through the play history and snapshot updates.

---

# 🛠️ Game Error Log

| # | Description                                                              | Turn / Snapshot                                    | Resolution / Notes                                                                                                                          |
| - | ------------------------------------------------------------------------ | -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| 1 | Confusion about **drive direction** after turnovers and snapshot changes | Resume snapshot (Quarter 2, 3rd & 2, Ball (15, L)) | Clarified: forward/backward is always toward the goal; lateral moves do **not** count toward progress.                                      |
| 2 | Miscalculation of ball position after last Play 4 (Breakaway)            | 3rd & 2 → 4 Red, 2 right                           | Initial assumption treated lateral as part of forward; corrected to row movement for forward and column for lateral → final ball `(10, N)`. |
| 3 | First down status not updated immediately after +5 step gain             | Same play                                          | Corrected: +5 forward exceeded 2 yards to first down → resets to 1st & 10.                                                                  |
| 4 | Confusion over previous “horizontal vs vertical” drive                   | During Play 4 resolution                           | Clarified: all forward/backward progress is along rows (toward goal). Lateral moves only columns.                                           |
| 5 | Previous board references `(32, J)` vs snapshot `(15, L)`                | Multiple references                                | Resolved by adopting the **Resume Snapshot as authoritative**. All subsequent calculations aligned with that.                               |
| 6 | Forward movement applied incorrectly on horizontal drive assumption      | Play 4 Red                                         | Corrected to vertical row changes for forward; lateral only affects column.                                                                 |
| 7 | Multiple overlapping snapshots / inconsistent downs                      | During game resumption                             | Standardized: after last Play 4, down resets to 1st & 10, quarter downs remaining updated.                                                  |
| 8 | Ambiguity about timeout protection                                       | During 3rd & 2 play                                | Clarified: timeout protection was **not used** for last play, down counting as normal.                                                      |

---

### ✅ Notes / Recommendations

1. **Always use the latest Resume Snapshot** as authoritative when resuming or calculating moves.
2. Track **blocked squares** explicitly in snapshots to avoid illegal moves.
3. Forward/backward should **always be along the rows toward goal**, lateral along columns only.
4. After gaining a first down, reset **Down = 1st & 10**, update **yards to next first down = 10**, and subtract one from **Quarter Downs Remaining**.
5. Keep a **timeout protection flag** in each snapshot to prevent accidental consumption of a down.

---



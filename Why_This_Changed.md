# Why This Changed — Developer Notes

> **Related Documents:**
>
> * See **CHANGELOG.md** for a chronological list of rule updates and version history
> * See **rules.md** for the current, authoritative ruleset
> * Deprecated rules referenced here are formally recorded in **rules.md → Deprecated Rules**

This document explains **why major rules were changed, replaced, or clarified** over time. It is intended for maintainers, contributors, and future designers—not for players learning the game.

The goal of these changes is to improve:

* Strategic depth
* Spatial clarity
* Fairness and balance
* Rules determinism (fewer edge-case disputes)

---

## 1. Direction of Play After Turnovers

**What changed:**

* Direction of play now reverses on a turnover while the ball remains at the turnover square.

**Why:**
Early versions allowed the ball to continue toward the same goal line after a turnover. This caused confusion about which team was attacking and undermined the concept of defending a goal.

**Design intent:**

* Make possession and direction intuitive
* Mirror real football logic
* Eliminate ambiguous scoring scenarios

---

## 2. Blocking Squares

**What changed:**

* Any square the ball passes through becomes blocked and cannot be reused.

**Why:**
Without blocking squares, optimal paths emerged quickly and plays became repetitive. Blocking squares force spatial planning and make lateral movement meaningful.

**Design intent:**

* Encourage creative routing
* Prevent infinite reuse of strong paths
* Add long-term board state consequences

---

## 3. Introduction of Colors & Match Logic

**What changed:**

* Added color selection layered on top of play numbers
* Introduced three match cases (full match, play-only, color-only)

**Why:**
Play-number guessing alone produced binary outcomes. Colors introduce partial information, bluffing, and graduated results.

**Design intent:**

* Increase mind-game depth
* Avoid all-or-nothing play resolution
* Reward prediction without making it absolute

---

## 4. Lateral Movement Overhaul

**What changed:**

* Lateral movement centralized into a dedicated rules section
* Explicit order of operations: lateral first, then forward/backward

**Why:**
Earlier rules described laterals piecemeal, leading to disputes about timing and legality.

**Design intent:**

* Make movement deterministic
* Remove table arguments about resolution order
* Clarify which plays truly support lateral strategy

---

## 5. Reduced Lateral Penalty on Defensive Match

**What changed:**

* Defense matching the play number now reduces lateral allowance by 1 instead of eliminating it entirely

**Why:**
A full lateral shutdown was overly punishing and collapsed spatial play. Reducing laterals preserves defensive reward without killing offense creativity.

**Design intent:**

* Keep laterals relevant
* Maintain balance between prediction and execution
* Preserve board navigation as a core skill

---

## 6. Kickoffs, Punts, and Return Distances

**What changed:**

* Kickoffs and punts standardized from the kicking team’s goal line
* Return distances shortened
* Added instant-touchdown check for no-match cases

**Why:**
Early returns were too long and low-risk, minimizing defensive impact and field-position strategy.

**Design intent:**

* Emphasize field position
* Make special teams meaningful but volatile
* Add high-risk/high-reward moments

---

## 7. Touchbacks

**What changed:**

* Automatic touchbacks for kicks past the end zone
* Optional touchbacks for kicks entering but not passing the end zone

**Why:**
Forced returns from deep positions created unfair disadvantages and slowed play resolution.

**Design intent:**

* Speed up gameplay
* Give receiving team agency
* Match real football expectations

---

## 8. Timeouts and Down Accounting

**What changed:**

* Timeouts prevent the next down from counting against the quarter limit

**Why:**
Without this, timeouts were strategically weak and often wasted.

**Design intent:**

* Make timeouts tactically valuable
* Encourage clock and down management

---

## 9. Quarter-End Warnings

**What changed:**

* Added a 4-down warning in the 2nd and 4th quarters

**Why:**
Players were being surprised by quarter ends, reducing meaningful planning.

**Design intent:**

* Improve transparency
* Support end-of-half strategy

---

## 10. Deprecated Rules Tracking

**What changed:**

* Deprecated rules are now documented and version-tagged

**Why:**
Rules evolved quickly, and undocumented removals caused confusion.

**Design intent:**

* Preserve institutional memory
* Support contributors
* Make future revisions safer

---

## Final Note

This game is intentionally treated as a **living ruleset**. Changes are made to improve clarity, fairness, and strategic depth—not to chase realism or complexity for its own sake.

If a rule changed, it changed for a reason.

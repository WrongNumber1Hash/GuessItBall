# Changelog

All notable changes to this game ruleset are documented in this file.

The format follows a simple versioning scheme:

* **Major version (1.x)**: Core ruleset era
* **Minor version (+0.1)**: Rule additions, clarifications, or balance changes
* Versions are cumulative unless explicitly stated otherwise

---

## **v1.0 — Original Ruleset**

**Initial release**

* Introduced grid-based football game (Columns A–T, Rows 1–64)
* Defined **goal lines** at Rows **5** and **59**
* Established **4 offensive plays** with base movement rules:

  * Play 1: Power / Sweep
  * Play 2: Interior Run
  * Play 3: Speed / Positioning
  * Play 4: Breakaway (available after Q1)
* Defense chooses a play number to counter the offense
* Forward/backward movement resolved by correct or incorrect defensive guess
* No color system
* No blocking squares
* No quarters, downs, or kickoffs

---

## **v1.1 — Quarters, Downs, and Direction**

* Added **4 quarters**
* Each quarter contains **15 downs**
* Introduced **goal direction** for each team
* Teams **switch ends after the 1st and 3rd quarters**
* Defined that **turnovers reverse direction**, but the ball stays in place

---

## **v1.2 — Blocking Squares**

* Added **blocking squares**
* Any square previously passed through becomes **blocked**
* Plays may not pass through blocked squares
* Offense must plan lateral or forward movement to avoid blocks
* Players may ask whether a square is blocked before a play resolves

---

## **v1.3 — Color System & Match Logic**

* Added **color selection** (Yellow / Red / Green)
* Introduced **three match cases**:

  * Full match (play + color) → turnover
  * Play-number match → negative or reduced movement
  * Color-only match → fixed forward movement
* Color logic layered **on top of base play rules**

---

## **v1.4 — Kickoff Rules**

* Added **kickoffs**:

  * Kickoff distance measured from the kicking team’s goal line
  * Receiving team selects **position (L/C/R)** and **color**
  * Kicking team selects the same
* Return distance based on number of matches
* No-match case triggers **1–10 number check** for instant touchdown

---

## **v1.5 — Lateral Kickoff Adjustment**

* Added lateral kickoff movement:

  * Kicking or receiving team may shift the result **5 steps left or right**
  * Who moves depends on who selected L or R
* Kickoff play ends if the ball goes out of bounds

---

## **v1.6 — Touchbacks & End Zone Rules**

* Added **touchback rule**:

  * If a kick goes past the end zone → automatic touchback
  * Ball placed at **Row 15, Column K**
* If a kick enters but does not pass the end zone:

  * Receiving team may choose a touchback after seeing the result

---

## **v1.7 — Timeouts**

* Added **timeouts**
* A timeout causes the **next down not to count** against the 15-down quarter limit
* Timeout count tracked per half

---

## **v1.8 — Coin Toss & Possession**

* Added **opening coin toss**:

  * Players choose heads or tails
  * Winner chooses to kick or receive
* At the start of the **2nd half**, the player who lost the opening toss chooses
* Kickoff rules apply to all half openings

---

## **v1.9 — Punt Plays**

* Added **punt option** as a legal play
* Punt follows kickoff-style resolution:

  * Position + color selection
  * Match-based return distance
  * No-match case triggers instant TD check
* Punt result square becomes **blocked**
* Receiving team begins with **1st down** after the return

---

## **v2.0 — Lateral Movement Overhaul**

**Major balance update**

* Centralized all lateral logic into **Section 8**
* Clarified that:

  * Lateral movement is only allowed if the play explicitly permits it
  * Lateral movement occurs **before** forward/backward resolution
* Reinforced blocked-square and out-of-bounds restrictions

---

## **v2.1 — Lateral Reduction on Defensive Play Match**

* Updated lateral rules:

  * When the **defense correctly matches the play number**, lateral movement is still allowed
  * Maximum lateral steps are reduced by **1**
* Formula introduced:

  > Adjusted laterals = Base laterals − 1
* Explicitly exempted:

  * Play 2 (never allows laterals)
  * Play 3 matched-play case (still forbids laterals entirely)

---

## **v2.2 — Quarter Warnings**

* Added **quarter-end warning**
* For **2nd and 4th quarters**, a warning is announced **4 downs before the quarter ends**

---

## **v2.3 — Rules Cleanup & Documentation**

* Clean rewrite of `rules.md`
* Separated:

  * Base play rules
  * Match modifiers
  * Movement rules
  * Special teams
* Prepared ruleset for public GitHub release

---


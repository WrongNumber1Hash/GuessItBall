# Examples

This document provides **worked examples** drawn directly from an actual played game using the current locked ruleset. Its purpose is to show *how rules resolve in practice*, especially for new players.

These examples assume familiarity with the glossary. All terms are used exactly as defined in **rules.md** and **GLOSSARY.md**.

---

## Sample Play 1 — Standard Offensive Play (Defense Chooses Wrong)

**Game state**

* Quarter: 2
* Down: 1st & 10
* Ball position: (36, K)
* Drive direction: toward Row 5

**Offense declares**

* Play: **4 — Breakaway**
* Color: **Black**
* Intended path: 2 steps right, then forward

**Defense declares**

* Play: **2**
* Color: **Red**

**Resolution**

* Defense guessed the wrong play number → *Defense chooses wrong*
* Base movement for Play 4 applies: **+5 forward**
* Play 4 allows up to 2 lateral steps → lateral move of 2 right is legal
* Lateral movement resolves first, then forward movement

**Result**

* Ball moves 2 columns right, then 5 rows forward
* All traversed squares become **blocked**
* Down advances by 1

---

## Sample Play 2 — Defensive Play Match with Reduced Lateral

**Game state**

* Quarter: 2
* Down: 3rd & 4
* Ball position: (21, L)
* Drive direction: toward Row 5

**Offense declares**

* Play: **1 — Power / Sweep**
* Color: **Black**
* Intended path: 2 steps right

**Defense declares**

* Play: **1**
* Color: **Red**

**Resolution**

* Defense correctly matches the play number
* Base Play 1 matched-play result: **no forward or backward movement**
* Play 1 normally allows 3 lateral steps
* Defensive match reduces lateral allowance by 1 → **2 laterals allowed**

**Result**

* Ball moves 2 steps right only
* No forward progress is made
* New square becomes blocked
* Down advances

---

## Sample Kickoff

**Situation**

* Start of the second half
* Kicking team’s goal line: Row 59

**Receiving team chooses**

* Position: **Center**
* Color: **Green**

**Kicking team chooses**

* Position: **Center**
* Color: **Green**

**Match evaluation**

* Position match: yes
* Color match: yes
* Total matches: **2**

**Kickoff result**

* Kick travels 20 steps from the kicking team’s goal line
* Return distance for 2 matches: **5 steps**
* No lateral adjustment chosen

**Result**

* Ball placed 5 steps forward from the return point
* Final square becomes blocked
* Receiving team starts **1st down**

---

## Sample Turnover (Full Match)

**Game state**

* Quarter: 2
* Ball position: (24, J)
* Drive direction: toward Row 5

**Offense declares**

* Play: **3 — Speed / Positioning**
* Color: **Red**

**Defense declares**

* Play: **3**
* Color: **Red**

**Resolution**

* Defense matches both play number and color → **full match**
* Full match triggers a **turnover**

**Turnover effects**

* Ball remains at (24, J)
* Possession changes
* **Drive direction reverses immediately**
* No movement occurs

**Result**

* New offensive player begins their drive from the same square
* Direction toward the opposite goal line is now considered forward

---

## ASCII Board Diagram Example

The diagram below illustrates a simplified slice of the board to demonstrate **positioning, movement, and direction**. This is not the full field.

```
Columns:   I   J   K   L   M
         -------------------
Row 25 |   .   .   B   .   .
Row 24 |   .   X   X   .   .
Row 23 |   .   .   .   .   .
Row 22 |   .   .   .   .   .
Row 21 |   .   .   .   .   .

Legend:
B = Ball position
X = Blocked square
. = Empty square
↑ = Forward direction (toward opponent’s goal line)
```

**Current state**

* Ball at **(25, K)**
* Drive direction: **upward (↑)**
* Blocked squares at **(24, J)** and **(24, K)**

---

### Example Movement

**Offense declares:**

* Play 1 — Power / Sweep
* Intended movement: 1 step right, then forward

**Resolution:**

* Lateral move from **K → L** is legal
* Forward movement from **(25, L) → (24, L)** is legal
* Ball may not move through blocked squares

**Resulting position:**

* Ball ends at **(24, L)**
* Squares **(25, K)**, **(25, L)**, and **(24, L)** become blocked

This diagram demonstrates:

* How blocked squares constrain routing
* How lateral movement avoids blocked paths
* How drive direction defines "forward"

---

## Why These Examples Matter

These scenarios demonstrate:

* Order of operations (lateral before forward)
* Defensive match effects
* Reduced lateral allowances
* Kickoff resolution
* Turnover handling and direction reversal

If a rules interaction is unclear, compare it against the closest example here.

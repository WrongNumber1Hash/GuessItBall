# Glossary

This glossary defines key terms used throughout **rules.md**, **CHANGELOG.md**, and **WHY_THIS_CHANGED.md**. These definitions are authoritative and intended to eliminate ambiguity during gameplay and rules interpretation.

---

## Forward / Backward

**Forward**

* Movement **toward the opponent’s goal line** the active player is attacking.
* The direction considered "forward" depends on:

  * Which goal line the player is currently driving toward
  * Whether teams have switched ends (after the 1st and 3rd quarters)

**Backward**

* Movement **away from the opponent’s goal line**, toward the player’s own goal line.
* Backward movement can result from:

  * Defensive play-number matches
  * Certain color or match outcomes

> Forward and backward are always evaluated relative to the **current drive direction**, not absolute board orientation.

---

## Blocked Square

A **blocked square** is any grid square that the ball has previously **passed through or landed on** during gameplay.

* Blocked squares:

  * ❌ Cannot be entered, passed through, or landed on
  * ❌ Cannot be used for lateral or forward movement
* Blocking applies immediately after a play resolves
* Blocked squares persist for the remainder of the game

**Purpose:**

* Prevents repeated use of optimal paths
* Forces spatial planning and creative routing

---

## Match vs. Color Match

These terms describe how defensive guesses interact with offensive choices.

### Match (Play Match)

A **match** occurs when the defense correctly guesses the **offensive play number**.

Effects may include:

* Reduced or negative forward movement
* Modified lateral allowances
* Turnover checks (depending on additional rules)

This is sometimes referred to as a **play-number match**.

---

### Color Match (Color-Only Match)

A **color match** occurs when:

* The defense correctly guesses the **offensive color**,
* But does **not** correctly guess the play number.

Effects:

* Ignores the base play’s normal result
* Applies a fixed forward movement defined by the color-match rules

> A color-only match is distinct from a full match and has its own resolution logic.

---

### Full Match

A **full match** occurs when the defense correctly guesses **both**:

* The offensive play number
* The offensive color

Effects:

* Usually triggers a **turnover**, unless otherwise specified by a special rule

---

## Drive Direction

**Drive direction** defines which goal line a player is currently attempting to reach.

* Each player always drives toward the **opposite goal line** from their own
* Drive direction:

  * Switches after the **1st and 3rd quarters**
  * **Immediately reverses on a turnover**
* The ball’s **position stays the same** on a turnover; only direction changes

Drive direction determines:

* What counts as forward vs backward
* How scoring is evaluated
* How movement is resolved

---

---

## Additional Terms for Non–American Football Players

The following terms are included to ensure the game is understandable without prior knowledge of American football.

---

## Down

A **down** is a single turn of play.

* Each play uses **one down** unless protected by a timeout
* A set of downs represents a limited number of attempts to advance the ball
* Each quarter contains **15 downs** total

---

## First Down (1st & 10)

A **first down** represents a reset of attempts.

* The offense starts at **1st & 10**, meaning:

  * 10 forward steps are required to earn another first down
* Gaining 10 forward steps:

  * Resets the down count
  * Establishes a new line to gain

This system prevents endless possession without progress.

---

## Line to Gain

The **line to gain** is an imaginary reference point:

* Located **10 forward steps** from the start of the current downs
* Crossing or reaching it awards a **first down**

It is not a physical board line but a tracking reference.

---

## Turnover

A **turnover** occurs when possession of the ball switches to the other player.

Turnovers may occur due to:

* Full play + color matches
* Certain color-only match checks
* Special teams outcomes

On a turnover:

* Ball position remains fixed
* **Drive direction immediately reverses**
* The opposing player begins their drive

---

## Possession

**Possession** indicates which player is currently controlling the ball and taking offensive actions.

* Only the player with possession may move the ball
* Possession changes via:

  * Turnovers
  * Kickoffs
  * Punts
  * Scoring plays

---

## Quarter

A **quarter** is a fixed segment of the game.

* The game consists of **4 quarters**
* Each quarter contains **15 downs**
* Teams switch ends after the **1st and 3rd quarters**

Quarters regulate pacing rather than time.

---

## Kickoff

A **kickoff** is a special play used to start:

* The game
* The second half
* Play after a touchdown

During a kickoff:

* The ball is advanced automatically from the kicking team’s goal line
* Position and color choices determine the return result

---

## Punt

A **punt** is a voluntary special play used to give up possession in exchange for better field position.

* The kicking team chooses to punt instead of running a normal play
* The ball advances 20 steps from the kicking team’s goal line
* Possession transfers to the receiving team after resolution

---

## Touchback

A **touchback** is a reset that occurs when a kick travels too deep into the end zone.

* The ball is placed at a predefined safe position
* The receiving team begins a new drive

This prevents unfairly poor starting positions.

---

## End Zone

The **end zone** is the scoring area beyond each goal line.

* Entering the opponent’s end zone with the ball scores a touchdown
* End zones do not create blocked squares for scoring purposes

---

## Touchdown

A **touchdown** is the primary scoring method.

* Occurs when the ball enters the opponent’s end zone
* May also occur via special instant-score conditions

---

## Lateral Movement

**Lateral movement** is horizontal movement across the board.

* Occurs left or right
* Always resolved **before** forward or backward movement
* Only allowed if the chosen play permits it

---

## Special Teams

**Special teams** refers to plays that are not standard offensive runs:

* Kickoffs
* Punts

These plays use separate resolution rules.

---

## Timeout

A **timeout** is a limited-use pause that alters down accounting.

* Using a timeout causes the next down **not to count** against the quarter limit
* Timeouts are strategic resources

---

## Final Note

If a term is capitalized in the rules and not defined elsewhere, it should be interpreted according to this glossary. In case of conflict, **rules.md** takes precedence, followed by this glossary.

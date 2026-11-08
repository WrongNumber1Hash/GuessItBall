# 🏈 GuessIT Ball: Turn-Based Grid Football

### *Official Comprehensive Manual & Strategy Guide*

A strategic football game played on a grid where players secretly select plays simultaneously. Manage physical fatigue, exploit positional skill mismatches, navigate a dynamically blocking field, and outguess your opponent. Customize your game with specialized roster builds and multiple field sizes.

---

## 🏗️ Section 1: Game Setup & Roster Creation

### 1.1 The 100-Point Roster Pool

Each team has **100 points** to distribute across 10 distinct position groups across Offense, Defense, and Special Teams. Points are split into two baselines:

* **Max Skill:** Determines the performance threshold of that position group on the field.
* **Max Stamina:** Determines the physical endurance and depth of that position group.

### 1.2 Official Team Roster Template

Players must allocate all 100 points prior to kickoff. Values chosen at the beginning of the game represent the Maximum Cap and can never be exceeded during play.

| Unit / Position Group | Max Skill | Max Stamina |
| --- | --- | --- |
| **🏈 OFFENSE** |  |  |
| 🔹 Offensive Line (OL) |  |  |
| 🔹 Quarterback (QB) |  |  |
| 🔹 Running Back (RB) |  |  |
| 🔹 Wide Receivers (WR) |  |  |
| **🛡️ DEFENSE** |  |  |
| 🔹 Defensive Line (DL) |  |  |
| 🔹 Linebackers (LB) |  |  |
| 🔹 Safeties (S) |  |  |
| 🔹 Cornerbacks (CB) |  |  |
| **👟 SPECIAL TEAMS** |  |  |
| 🔹 Kick Off / Punt (KO/P) |  |  |
| 🔹 Kick / Punt Return (KR/PR) |  |  |
| **TOTALS** | **/ 100 Points Total** |  |

---

## 🗺️ Section 2: Field Options & Game Structure

Players must agree on the field dimensions and game length mode prior to the opening coin toss.

### 2.1 Field Dimension Options

#### 📐 Option 1: The Standard Grid (64 Rows)

* **Grid Size:** Columns A–T, Rows 1–64.
* **Goal Lines:** Row 5 (Team A) and Row 59 (Team B).
* **End Zones:** Rows 1–5 and Rows 59–64 (5 rows deep).

#### 📐 Option 2: The Expanded Field (120 Rows)

* **Grid Size:** Columns A–T, Rows 1–120.
* **Team A End Zone:** Rows 1–10 (10 rows deep).
* **Team A Goal Line:** Row 11.
* **The Playing Field:** Rows 11–110 (Exactly 100 playable spaces/yards).
* **Team B Goal Line:** Row 110.
* **Team B End Zone:** Rows 111–120 (10 rows deep).

### 2.2 Game Length Options

#### 🏁 Option A: The 10-Down Quickplay Blitz

* **Length:** The entire game lasts a maximum of 10 total downs from the opening kickoff.
* **Play 4 Unlocked:** Because it is an intense, fast-paced sprint, Play 4 (*Breakaway*) is unlocked right from Down 1.
* **Turnover Reset:** A turnover instantly awards a fresh set of downs to the recovering team, resetting their drive count back to Down 1. The total 10-down game clock continues to tick.
* **Victory Condition:** The first team to cross the goal line and score a touchdown wins the game instantly.

#### ⏱️ Option B: Regulation Play (Full Game Setup)

* **Length:** A full game consists of 4 quarters, with each quarter lasting 15 downs (60 total downs per game).
* **Play 4 Locked:** To build tension, Play 4 (*Breakaway*) is locked during Quarter 1 and only becomes available starting on Down 16 (Quarter 2).
* **Standard Football Series:** Teams have a standard 4 downs to gain 10 forward rows to achieve a First Down. Failing to gain 10 rows results in a turnover on downs, forcing a punt, or attempting a field goal.
* **Victory Condition:** The team with the highest point total at the end of the 4th quarter wins.

### 2.3 Permanently Blocked Squares

Every play's ending coordinate becomes a **permanently blocked square 🟥** for the rest of the game.

* No player moving on the ground may enter or pass through a blocked square.
* Physical blockades force teams to strategically utilize lateral movement or the passing game to navigate the field.

---

## 👟 Section 3: Special Teams Mechanics

### 3.1 Kickoff Execution

* **Standard Grid Setup:** The kickoff baseline travels 55 rows downfield from the kicking team's goal line (landing on Row 60).
* **Expanded Field Setup:** The kickoff baseline travels 75 rows downfield from the kicking team's goal line (landing on Row 86 from Row 11, or Row 35 from Row 110).
* **The Special Teams Skill Check:** Prior to resolution, compare the Kicking Team's **KO/P Skill** against the Receiving Team's **KR/PR Skill**.
* **If KO/P Skill is higher:** The ball travels an additional 5 rows downfield.
* **If KR/PR Skill is higher:** The receiving team adds +5 rows to their final return distance.
* **If Tied:** No distance bonuses are awarded.



### 3.2 Kickoff Return Matrix

Both players simultaneously declare a Position (**Left / Center / Right**) and a Color (**Yellow / Red / Green**). The return distance is based on defensive matches:

* **2 Matches:** Kickoff returned exactly 5 steps.
* **1 Match:** Kickoff returned exactly 10 steps.
* **0 Matches:** Kickoff returned 15 steps + **Instant TD Number Check** *(Both pick a number 1–10; a perfect match scores an immediate touchdown)*.

---

## 🎮 Section 4: How To Play Each Down

### 4.1 Play Locking Phase

Both players secretly lock in their choices simultaneously:

* **Offense Declares:** Play Number (1–4), Color (Red/Black), and Lateral Movement Intent.
* **Defense Declares:** Play Number (1–4) and Color (Red/Black).

### 4.2 The 4 Core Plays & Spatial Resolution

* **🟦 Play 1 – Power/Sweep (Safe Run)**
* *Defense Wrong:* +4 forward, up to 3 lateral allowed.
* *Defense Matches:* 0 forward, up to 2 lateral allowed.


* **🟩 Play 2 – Interior Run (Linear Attack)**
* *Defense Wrong:* +2 forward, no lateral allowed.
* *Defense Matches:* -2 backward, no lateral allowed.


* **🟨 Play 3 – Speed/Positioning (Spatial Finesse)**
* *Defense Wrong:* +1 forward, up to 3 lateral allowed.
* *Defense Matches:* -3 backward, no lateral allowed.


* **🟥 Play 4 – Breakaway (The Juggernaut)**
* *Defense Wrong:* +5 forward, up to 2 lateral allowed.
* *Defense Matches:* -4 backward, up to 1 lateral allowed.



### 4.3 Color Selection & Environmental Interaction

* **🔴 Red (Pass):** Air Mechanics. Lateral movement designated as "Before" or "After" forward movement. Air movement completely ignores blocked squares, but ground movement is stopped by them.
* *Before:* Lateral = Air (ignores blocks) | Forward = Ground (blocked).
* *After:* Forward = Air (ignores blocks) | Lateral = Ground (blocked).


* **⚫ Black (Run):** Ground Mechanics. All movement occurs along the turf. If the ball's path hits a blocked square at any point, the play stops immediately on the square prior.

### 4.4 Defensive Match Matrix

| Match Result | Mechanical Outcome |
| --- | --- |
| **No Match** | Apply base play result (Defense Wrong) + 2 Bonus Forward Steps. |
| **Play Match Only** | Apply matched play result + 2 Bonus Forward Steps. Lateral movement capability is reduced by 1. |
| **Color Match Only** | Ignore play result. Move exactly +3 Forward. Both teams pick a number 1–10 (A match causes a turnover). |
| **Play + Color Match** | 🚨 **IMMEDIATE TURNOVER.** Ball stays in place, drive direction completely reverses, and downs reset to Down 1. |

### 4.5 Movement Terminology

* **Forward:** Movement toward the opponent's goal line.
* **Backward:** Movement away from the opponent's goal line.
* **Lateral:** Movement left or right across columns. Default occurs *before* forward movement if not specified.

---

## ⚡ Section 5: Live Skill Checks

On every down where a Play + Color Match Turnover does not occur, the live current Skill stats are computed to determine performance bonuses.

### 5.1 Positional Pair Skill Check (+2 Yards)

Add the current Skill points of the two relevant position groups dictated by the play type. If the Offense's total is strictly higher than the Defense's total, the offense gains a **+2 Forward Yard Bonus**.

* **🟦 Play 1 & 🟩 Play 2 (Run Battles):** Offense (OL + RB) vs. Defense (DL + LB)
* **🟨 Play 3 & 🟥 Play 4 (Space Battles):** Offense (QB + WR) vs. Defense (CB + S)

### 5.2 Overall Team Skill Check (+1 Yard)

Compare the total combined active Skill score of all four offensive groups on the field against all four defensive groups. If the offense has a higher total team skill than the defense, they earn a **+1 Forward Yard Bonus**.

---

## 🔋 Section 6: Active Resource Management Loop

Physical endurance fluctuates constantly based on utilization. At the end of every active down, resource adjustments must be calculated before proceeding to the next snap.

### 6.1 The Active Depletion & Replenishment Choice

The active player on the field must choose **exactly one** position group to shoulder the fatigue of the down:

* The chosen group's **Current Stamina** depletes by **2**.
* The chosen group's **Current Skill** replenishes by **2** (up to its maximum assigned cap).
* *Note: All other active groups on the field remain at their current stamina and skill levels.*

### 6.2 Sideline Recovery Rule

Units resting on the sideline get to catch their breath:

* While a player's **Defense** is on the field, all 4 of their **Offensive** position groups recover **+2 Stamina** at the end of the down (up to their maximum cap).
* Conversely, while a player's **Offense** is on the field, all 4 of their **Defensive** position groups recover **+2 Stamina**.

---

## 🎯 Section 7: Scoring & After-Touchdown Conversions

A **Touchdown (6 Points)** is scored the exact moment the ball crosses the plane and enters the opponent's 10-row deep (or 5-row deep) end zone. The scoring team can choose one of two options to complete their drive:

### 7.1 The 1-Point Extra Point (Kicking Game)

The scoring player attempts a placekick.

1. **Compare Special Teams Skills:** If the defending team's KR/PR Skill is strictly higher than the kicking team's KO/P Skill, the defense selects 2 numbers from 1–10. Otherwise, the defense selects 1 number from 1–10.
2. The defense secretly locks in their block number(s).
3. The kicking player guesses a number from 1–10.
* **Match:** The kick is **Blocked**. Score remains at 6 points.
* **No Match:** The kick is **Good!** Score becomes 7 points.


### 7.2 The 2-Point Conversion (Scrimmage Play)

The offense places the ball on the 2-space line relative to the goal line and runs a single, high-stakes standard down. Both sides lock in a play number and color.

* **Placement (Standard):** Row 57 (driving toward Row 59).
* **Placement (Expanded):** Row 13 (driving toward Row 10) or Row 108 (driving toward Row 111).
* **Resolution:** If the offense resolves the play with a net movement of 2 or more forward rows, the conversion is successful, awarding **2 points** (8 points total).
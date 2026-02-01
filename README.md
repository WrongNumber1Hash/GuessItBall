# GuessItBall

---

# 🏈 Turn-Based Grid Football Game

A **turn-based, strategy football game** played on a grid.
Players secretly choose plays, manage space, avoid blocked squares, and out-think their opponent across four quarters.

This can be played by 2-6 players, with more players taking turns as coach, being able to deploy different plays (offense or defense) or customize their play results.

🚀 Quick Start (Chat Setup)

New to the game? Start with [Quick Start: Chat Setup](quick_start_new_chat.md).

This one-page guide explains how to initialize a game in chat — coin toss, kickoff choice, play locking, starting orientation, and the first snap — so you can begin playing in under a minute, even without reading the full rules.

---

## 🧩 The Board

* **Columns:** A–T
* **Rows:** 1–64
* **Goal lines:**

  * One team scores at **Row 5**
  * The other scores at **Row 59**

Each square represents one step.
When a square is used by a play, it becomes **blocked** and cannot be used again.

---

## 🔄 How a Turn Works

Each down follows this sequence:

1. **Play is locked**
2. Both players secretly choose:

   * A **Play** (1–4)
   * An optional **Color**
3. Offense declares a **path** (lateral first, then forward/backward)
4. Plays are revealed
5. Movement is resolved using:

   * Base play rules
   * Match & color rules
6. The final square becomes **blocked**
7. Down advances (unless protected by timeout)

---

## 🎯 Offensive Plays (Overview)

| Play  | Style                | Risk        |
| ----- | -------------------- | ----------- |
| **1** | Power / Sweep        | Low         |
| **2** | Interior Run         | Medium      |
| **3** | Speed / Positioning  | Medium–High |
| **4** | Breakaway (after Q1) | High        |

Each play has different forward, backward, and lateral rules depending on whether the defense guesses correctly.

---

## 🎨 Match & Color System

After the base play resolves:

* **No match:** Bonus forward movement
* **Play match only:** Reduced or backward result + small bonus
* **Color match only:** Fixed forward gain + turnover check
* **Play + color match:** **Turnover**

Turnovers reverse the direction of play but keep the ball where it is.

---

## ⏱️ Game Structure

* **4 quarters**
* **15 downs per quarter**
* **Warnings** in the 2nd & 4th quarters (4 downs remaining)
* Teams **switch ends** after Q1 and Q3
* Timeouts protect a down from counting against the quarter limit

---

## 🦵 Kickoffs, Punts & Touchbacks

* Kickoffs and punts use **position + color guessing**
* Match results determine return distance
* Some outcomes trigger **instant touchdown checks**
* Kicks past the end zone = **touchback at Row 15, Column K**
* Final return square becomes **blocked**

---

## 🧠 Why This Game Is Different

* Space permanently changes due to blocked squares
* Risk compounds over time
* Every rule interaction matters
* Players are rewarded for **anticipating tendencies**, not randomness

Think **chess meets football**.

---

## 📘 Where to Go Next

* 👉 **Full rules:** [`rules.md`](rules.md)
* 👉 **Variants:** [`anywhere_variant.md`](anywhere_variant.md)
* 👉 **Design notes:** [`Ai_feedback.md`](Ai_feedback.md)
* 👉 **Translations:** `lang/`

---

## ⚖️ Status

This is a **living ruleset**.
Feedback, testing, and variants are welcome.

---


⚠️ WARNING: This game involves psychological interaction. Please read the Disclaimer before playing or contributing.

Games using emotion or psychology to engage players to interact with each other

The second game is *GuessItBall*, a game for between 2-6 people. Goal is to gain the most total yardage and/or points by the end of the game. Variants of the game without cards, and using different materials will also be posted and updated. This is based on the rules for American football, but have been customized. 

Players can modify the game by adding or removing rules, creating their own rules, or customizing parts to fit their own visions for the game. I will add an Anywhere variant that uses common playing cards as substitutes for the choosing the play number, and tokens for betting. There is an optional Bookie role to keep track of bets, tokens and the Bank.

Please read the **LICENSE** to see the details of the Creative Commons CC BY 4.0 license [Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).

Please see the **DISCLAIMER** for Liability Notice and Psychological Notice & Waiver of Liability.

Please view the **Code of Conduct** for an important notice for users to abide by certain rules.





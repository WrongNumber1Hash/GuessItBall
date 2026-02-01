# playtesting_with_ai.md

--

Before we kick off, we just need to lock **a few setup details** so the game runs cleanly in chat. I’ll keep this tight.

### Let’s confirm these 5 things:

1. **Who starts on offense?**

   * You offense / me defense
   * or me offense / you defense

2. **Win condition** (pick one for now):

   * First to reach the opponent’s end zone
   * OR highest total forward advancement after 4 quarters

3. **Quarter timing in chat**
   Since real-time minutes are messy here, I suggest:

   * Each quarter = **15 rounds only** (ignore the 10-minute rule)
     ✔️ Unless you want something different.

4. **Play secrecy method**
   To keep choices secret, we can do:

   * Both type: `Play locked`
   * Then reveal simultaneously in the next message
     (This works really well in turn-based chat.)

5. **Starting orientation**

   * Starting square confirmed as **(32, center width)**
   * Forward direction = increasing step numbers (toward 64)

If you reply with:

* Offense/Defense choice
* Win condition
* Any tweaks

…I’ll set up the **official game state** and we’ll snap the ball on **Down 1, Quarter 1** 🏈🔥

Got it — **you’re on offense** 🏈
I’m on defense.

---

## ✅ Game State Initialized

**Quarter:** 1
**Round:** 1
**Down:** 1 of 4
**Drive Progress:** 0 / 10
**Ball Position:** **(32, K)**
**Play 4:** ❌ Locked (available starting Quarter 2)
**Timeouts:** You 3 | Me 3

### 📒 Position Log

* Start: **(32, K)**

---

## 🔐 Play Selection Protocol (Locked In)

* We’ll use **simultaneous reveal**:

  1. You choose a play (1–3)
  2. I choose a defensive number (1–3)
  3. We both type **“Play locked”**
  4. Next message: **reveal**

---

### 👉 When ready:

Type **“Play locked”**
(That signals your play is chosen. I’ll do the same, then we reveal.)

Down 1. Ball is live. Let’s see if I can read you 😏

---


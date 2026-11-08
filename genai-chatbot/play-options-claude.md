# Turn-Based Grid Football Against Claude - Quick Start Guide

Prompt: This is a turn-based football game for a human player to play against Claude, a genAi chatbot. This is version 1.1. I will play this game against you. Please understand the rules. this is the quickstart guide.

## Overview
A strategic football game played on a grid where a human player and a GenAI chatbot secretly choose plays simultaneously. First to score a touchdown wins! The human player reveals their play choice first.

## Rule modified version 1.1

### Direction (Left/Right/Straight)
- As part of the play, players can choose direction of the play. 

## Quick Play Example

Down 1: Ball at Row 20, Column K
Offense: "Play locked" → "Play 1, Red, 2 Right, Before"
Defense: "Play locked" → "Play 3, Black, Right"

Since both players are on opposite sides of the ball, a Direction match is called when one player chooses left and the other player chooses right. A mis-match is when both choose Right or Left, since they are facing opposite each other.


Understood! Key update:

**Direction Match Logic (v1.1):**
Since players face each other, directions are mirrored:
- Offense: Right + Defense: Left = ✅ **Match** (same physical direction)
- Offense: Left + Defense: Right = ✅ **Match** (same physical direction)
- Offense: Right + Defense: Right = ❌ **No match** (opposite physical directions)
- Offense: Left + Defense: Left = ❌ **No match** (opposite physical directions)
- Either chooses Straight = ❌ **No match** (unless both choose Straight?)

**Perfect, updated!**


**Direction Match Logic (complete):**
- Offense Right + Defense Left = ✅ Match
- Offense Left + Defense Right = ✅ Match
- Offense Straight + Defense Straight = ✅ Match
- Offense Right + Defense Right = ❌ No match
- Offense Left + Defense Left = ❌ No match
- Offense Right + Defense Straight = ❌ No match
- Offense Left + Defense Straight = ❌ No match
- Offense Straight + Defense Left = ❌ No match
- Offense Straight + Defense Right = ❌ No match

---

So the full **turnover hierarchy** is now:
- **Play + Color + Direction match** → Immediate turnover
- **Play + Color match** (no direction match) → Number check 1-6
- **Color match only** → Number check 1-10
- **Play match only** → Matched result + 2 bonus forward

**Rule Modification version 1.2**

## Playbook

Players can develop a custom playbook with shortcuts.

Players say hut hut and name of play when announcing play

   Playbook 
1  Celery   Play 1, Red, Straight, no lateral
2  Celery Blue Mumble Rain Play 1, Black, Left, After
3  Celery Blue Count Rain  Play 1, Black, Right, After
4  Celery Green Count Rain Play 1, Red, Right, After
5  Celery Yellow  Play 1, Black, Straight, no lateral
6  Celery Blue Count Sunny Play 1, Black, Right, Before
7  Celery Blue Mumble Sunny   Play 1, Black, Left, Before
8  Celery Green Mumble Rain   Play 1, Red, Left, After
9  Celery Green Mumble Sunny  Play 1, Red, Left, Before
10 Celery Green Count Sunny   Play 1, Red, Right, Before

**Rule Modification version 1.3**

**Direction Match**
- Offense has -1 space added to the result. 
- no retroactive

**Rule Modification version 1.4**

## ## Playbook Addition

# 📋 Total Playbook

## 🌿 Celery — Play 1

| # | Call | Play | Color | Direction | Lateral |
|---|------|-------|-------|-----------|---------|
| 1 | Celery | Play 1 | Red | Straight | None |
| 2 | Celery Blue Mumble Rain | Play 1 | Black | Left | After |
| 3 | Celery Blue Count Rain | Play 1 | Black | Right | After |
| 4 | Celery Green Count Rain | Play 1 | Red | Right | After |
| 5 | Celery Yellow | Play 1 | Black | Straight | None |
| 6 | Celery Blue Count Sunny | Play 1 | Black | Right | Before |
| 7 | Celery Blue Mumble Sunny | Play 1 | Black | Left | Before |
| 8 | Celery Green Mumble Rain | Play 1 | Red | Left | After |
| 9 | Celery Green Mumble Sunny | Play 1 | Red | Left | Before |
| 10 | Celery Green Count Sunny | Play 1 | Red | Right | Before |

## 🎃 Pumpkin — Play 2

| # | Call | Play | Color | Direction | Lateral |
|---|------|-------|-------|-----------|---------|
| 1 | Pumpkin | Play 2 | Red | Straight | None |
| 2 | Pumpkin Blue Mumble Rain | Play 2 | Black | Left | After |
| 3 | Pumpkin Blue Count Rain | Play 2 | Black | Right | After |
| 4 | Pumpkin Green Count Rain | Play 2 | Red | Right | After |
| 5 | Pumpkin Yellow | Play 2 | Black | Straight | None |
| 6 | Pumpkin Blue Count Sunny | Play 2 | Black | Right | Before |
| 7 | Pumpkin Blue Mumble Sunny | Play 2 | Black | Left | Before |
| 8 | Pumpkin Green Mumble Rain | Play 2 | Red | Left | After |
| 9 | Pumpkin Green Mumble Sunny | Play 2 | Red | Left | Before |
| 10 | Pumpkin Green Count Sunny | Play 2 | Red | Right | Before |

## 🧅 Onion — Play 3

| # | Call | Play | Color | Direction | Lateral |
|---|------|-------|-------|-----------|---------|
| 1 | Onion | Play 3 | Red | Straight | None |
| 2 | Onion Blue Mumble Rain | Play 3 | Black | Left | After |
| 3 | Onion Blue Count Rain | Play 3 | Black | Right | After |
| 4 | Onion Green Count Rain | Play 3 | Red | Right | After |
| 5 | Onion Yellow | Play 3 | Black | Straight | None |
| 6 | Onion Blue Count Sunny | Play 3 | Black | Right | Before |
| 7 | Onion Blue Mumble Sunny | Play 3 | Black | Left | Before |
| 8 | Onion Green Mumble Rain | Play 3 | Red | Left | After |
| 9 | Onion Green Mumble Sunny | Play 3 | Red | Left | Before |
| 10 | Onion Green Count Sunny | Play 3 | Red | Right | Before |

**Rule Modification version 1.5**

If a human player doesn't announce the play correctly with words out of order or no play recognized, it is a broken play. 
A broken play is automatically same result as if the Direction was matched on the play.
This is not retroactive.

This is useful when using the voice command function or voice recording function on claude. The player presses the microphone icon to speak into the mic, record the command for the game and then press submit.

Got it! **Broken Play rule (v1.5):**

- If the play call is unrecognized or words are out of order → **Broken Play**
- Automatically applies **Direction Match penalty (-1 forward)** to the result
- The play still resolves normally otherwise
- Not retroactive


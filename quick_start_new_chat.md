# Turn-Based Grid Football - Quick Start Guide

## Overview
A strategic football game played on a grid where both players secretly choose plays simultaneously. First to score a touchdown wins!

## The Board
- **Grid**: Columns A-T, Rows 1-64
- **Goal Lines**: Row 5 (one team) and Row 59 (other team)
- **End Zones**: Rows 1-5 and Rows 59-64

## Game Setup

### 1. Coin Toss
- Winner chooses to **kick** or **receive**
- Loser gets choice at start of 2nd half

### 2. Kickoff
1. Kick travels 55 rows from kicking team's goal line
2. Both players choose:
   - **Position**: Left / Center / Right
   - **Color**: Yellow / Red / Green
3. Return distance based on matches:
   - 2 matches = 5 steps
   - 1 match = 10 steps
   - 0 matches = 15 steps + number check (1-10, match = TD!)

## How to Play

### Each Down (Turn)
1. Both players say **"Play locked"**
2. Offense reveals first: Play number, Color, Movement intent
3. Defense reveals: Play number, Color
4. Resolve the play
5. Mark the ending square as **blocked** (can't be entered again)

### The 4 Plays

**🟦 Play 1 - Power/Sweep**
- Defense wrong: +4 forward, up to 3 lateral
- Defense matches: 0 forward, up to 2 lateral

**🟩 Play 2 - Interior Run**
- Defense wrong: +2 forward
- Defense matches: -2 backward, no lateral

**🟨 Play 3 - Speed/Positioning**
- Defense wrong: +1 forward, up to 3 lateral
- Defense matches: -3 backward, no lateral

**🟥 Play 4 - Breakaway** (unlocked after Quarter 1)
- Defense wrong: +5 forward, up to 2 lateral
- Defense matches: -4 backward, up to 1 lateral

### Color Selection

**Red (Pass)**
- Movement through air ignores blocked squares
- Risk: Can go incomplete if overshooting end zone

**Black (Run)**
- Movement on ground - blocked squares stop you

### Match Results

**No Match**
- Apply base play result
- **+2 bonus forward steps**

**Play Match Only**
- Apply matched result
- **+2 bonus forward steps**

**Color Match Only**
- Ignore play result
- Move exactly **+3 forward**
- Both pick number 1-10 (match = turnover!)

**Play + Color Match**
- **IMMEDIATE TURNOVER**
- Ball stays in place
- Drive direction reverses

## Movement Rules

### Lateral Movement
- Declared as "before" or "after" forward movement
- Default is before if not specified
- Can go left or right across columns
- Reduced by 1 if defense matches play number

### Forward/Backward Movement
- Toward opponent's goal line = forward
- Away from opponent's goal line = backward

### Red (Pass) Movement
- **Before**: Lateral = air (ignores blocks), Forward = ground (blocked by blocks)
- **After**: Forward = air (ignores blocks), Lateral = ground (blocked by blocks)

### Black (Run) Movement
- All movement = ground (blocked squares stop you)

## Scoring

**Touchdown occurs when:**
- Ball enters opponent's end zone (5 rows deep)
- Instant TD on kickoff/punt number match

**First team to score wins the game!**

## Key Concepts

### Downs & First Downs
- Start at **1st & 10** (need 10 forward rows)
- Gain 10+ rows → Reset to 1st & 10
- 4 downs to make progress or punt

### Quarters
- 4 quarters, 15 downs each
- Switch ends after Quarter 1 and Quarter 3
- Warning at 4 downs remaining in Q2 and Q4

### Blocked Squares
- Every play ending position becomes blocked
- Cannot enter or pass through (except Red air movement)
- Strategic positioning matters!

### Turnovers
- Play + Color match = instant turnover
- Color match only = number check for turnover
- Ball stays where it is, drive direction reverses

## Quick Play Example

Down 1: Ball at Row 20, Column K
Offense: "Play locked" → "Play 1, Red, 2 right before"
Defense: "Play locked" → "Play 3, Black"

Result: No match!
- Base Play 1 (defense wrong): +4 forward, 3 lateral allowed
- Bonus: +2 forward
- Total: +6 forward, 2 lateral right

Movement: Row 20 → Row 26, Column K → Column M
New position: Row 26, Column M (now blocked)

## Tips for Beginners

1. **Mix up your plays** - Don't be predictable!
2. **Watch blocked squares** - They limit movement options
3. **Color match risk/reward** - Red passes can go further but risk turnovers
4. **Lateral movement** - Use it to avoid blocked squares
5. **Play 4 is powerful** - But only after Quarter 1

## Ready to Play?

1. Decide who kicks off (coin toss)
2. Resolve kickoff
3. Start calling plays!
4. First touchdown wins!

Good luck! 🏈

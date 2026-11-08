# Turn-Based Grid Football Against Claude - Quick Start Guide

Prompt: This is a turn-based football game for a human player to play against Claude, a genAi chatbot. This is version 1.1. I will play this game against you. Please understand the rules. this is the quickstart guide.

## Overview
A strategic football game played on a grid where a human player and a GenAI chatbot secretly choose plays simultaneously. First to score a touchdown wins! The human player reveals their play choice first.

## The Board
The Game board is represented by the following dimensions. It can be presented in ASCII text format with a prompt to Claude.
- **Grid**: Columns A-T, Rows 1-64
- **Goal Lines**: Row 5 (one team) and Row 59 (other team)
- **End Zones**: Rows 1-5 and Rows 59-64

Prompt: Print the game board and current ball position

## Game Setup

The human player should read the instructions and rules, because they will have to confirm that Claude is applying the rules correctly. Human players should refer to the rules when challenging any result announced by Claude that appears to violate the rules, or is a wrong interpretation of the rules. Players can copy and paste the rules into the chat window to reinforce any challenges to Claude.

### 1. Coin Toss

Claude handles the coin toss for the human player, and before flipping the coin, the human player chooses heads or tails. After the human player makes their choice, Claude flips the coin and announces the result. 

- Winner chooses to **kick** or **receive**
- Loser gets choice at start of 2nd half

### 2. Kickoff
1. Kick travels 55 rows from kicking team's goal line
2. Both players choose:
   - **Position**: Left / Center / Right
   - **Color**: Yellow / Red / Green

The human player announces their choices first and then the GenAI player reveals the choices they had made.

3. Return distance based on matches:
   - 2 matches = 5 steps
   - 1 match = 10 steps
   - 0 matches = 15 steps + number check (1-10, match = TD!)

## How to Play

### Each Down (Turn)
1. Both players say **"Play locked"**
2. Offense reveals first if Human Player : Play number, Color, Direction of Lateral movement, and before or after play
3. Defense reveals: Play number, Color, Direction of Counter play
4. Resolve the play
5. Mark the ending square as **blocked** (can't be entered again)

### The 4 Plays

**🟦 Play 1 - Power/Sweep**
- Defense wrong: +4 forward, up to 3 lateral
- Defense matches number: 0 forward, up to 2 lateral

**🟩 Play 2 - Interior Run**
- Defense wrong: +2 forward
- Defense matches number: -2 backward, no lateral

**🟨 Play 3 - Speed/Positioning**
- Defense wrong: +1 forward, up to 3 lateral
- Defense matches number: -3 backward, no lateral

**🟥 Play 4 - Breakaway** (unlocked after Quarter 1)
- Defense wrong: +5 forward, up to 2 lateral
- Defense matches number: -4 backward, up to 1 lateral

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
- The human player chooses a number between 1 and 6
- Human player announces their choice
- GenAI generates a random result between 1 and 6
- If the randomly generated number matches the human player's choice, then it is an immediate turnover
- The ball is turned over and the drive direction reverses. The Down resets to 1st down.

**Play + Color + Direction Match**
- **IMMEDIATE TURNOVER**
- Ball stays in place
- Drive direction reverses
- The Down resets to 1st down.

**Direction Match**
- Offense has -1 space added to the result. 

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

### Direction (Left/Right/Straight)
- As part of the play, players can choose direction of the play. 
- 

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
Offense: "Play locked" → "Play 1, Red, 2 Right, Before"
Defense: "Play locked" → "Play 3, Black, Right"

Since both players are on opposite sides of the ball, a Direction match is called when one player chooses left and the other player chooses right. A mis-match is when both choose Right or Left, since they are facing opposite each other.

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

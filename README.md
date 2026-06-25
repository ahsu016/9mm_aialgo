# 9mm_aialgo

# Nine Men's Morris AI

## Description

This is a simple AI for Nine Men's Morris.  
It uses a board representation, heuristic evaluation, and Minimax search to suggest moves.

---

## Board

The board has 24 positions:

```python
board = [None] * 24
```

Values:
- `None` = empty
- `"W"` = white
- `"B"` = black

---

## Key Features

- Legal move generation (placing, moving, flying)
- Mill detection
- Heuristic evaluation function
- Minimax move search

---

## Game Data

### ADJACENT

Defines valid moves between positions.

### MILLS

All possible three-in-a-row combinations.

---

## Heuristic

The AI evaluates positions using:

- Mills
- Piece count
- Potential mills
- Mobility (in moving phase)

Higher score = better position

---

## How it works

1. Generate legal moves
2. Simulate each move
3. Score positions using heuristic
4. Pick best move using Minimax

---

## Future improvements

- Alpha-beta pruning
- Capture handling after mills
- Better evaluation weights

# 2048-puzzle
A.I - Implemented Minimax algorithm with ab-pruning using iterative deepening to solve the 2048-puzzle. Each move selection should be under 0.1 seconds.

Injected 5 different heuristics with adjustable weights to evaluate moves:
```
smoothness (Αdjacent tiles should decrease in value but neighbor tiles should be close enough to potentially merge)
monotonicity (Values of the tiles should all either increasing or decreasing along both the left/right and up/down directions)
emptiness (Evaluate each move on the number of empty tiles it generates)
maxvalue (Maximum value of the generated tiles)
distance (Scalable distance from the upper-left corner of the grid)
```

## Usage
GameManager.py

## Results
The agent surpassed the goal of 2048 value tile and got to 4096. Probably with a minor change on strategy, maybe dynamically altering the heuristic weights, it may go even further.

![alt tag](http://www.supergramm.com/media/images/github/results.jpg)

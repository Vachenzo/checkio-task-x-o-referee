The enemy has lined up in our sights! Oh, this makes them a juicy target for our high-velocity gun.
We'll just have to set up the line detection.

Think back to the game Tic-Tac-Toe, sometimes also known as Xs and Os. This is a game for two players (X and O)
who take turns marking the spaces in a 3×3 grid.
The player who succeeds in placing three respective marks 
in a horizontal, vertical, or diagonal rows (NW-SE and NE-SW) wins the game.

But we will not be playing this game.
You will be the referee for this games results. 
You are given a result of a game and you must determine 
if the game ends in a win or a draw as well as who will be the winner. 
Make sure to return "X" if the X-player wins and "O" if the O-player wins. If the game is a draw, return "D".

![X-O](x-o-referee.svg)

A game's result is presented as a list of strings, where "X" and "O" are players' marks and "." is the empty cell.




**Input:**  A game result as a list of strings (unicode).

**Output:** "X", "O" or "D" as a string.


**Example:**

```python
referee([
    "X.O",
    "XX.",
    "XOO"]) == "X"
referee([
    "OO.",
    "XOX",
    "XOX"]) == "O"
referee([
    "OOX",
    "XXO",
    "OXX"]) == "D"
```

**How it is used:**

The concepts in this task will help you when iterating data types.
They can  also be used in game algorithms, allowing you to know how to check results.

**Precondition:**
```python
len(game_result) == 3
all(len(row) == 3 for row in game_result)
```

There is either one winner or a draw.


# tic_tac_toe-BOT

**A tic-tac-toe BOT program, that plays optimally to either win or draw a game.**

## There are two implementations:
- Naive Implementation(Using a set of fixed rules).
- Using the Minimax Algorithm along with alpha-beta pruning to increase efficiency.

Numpad is used to select the desired block which are numbered from 1 to 9 and in same relative order as on the numpad.

![image](https://github.com/sonuverma1/tic_tac_toe-BOT/blob/master/Numpad.jpg)
### Naive Implementation has the following rules:

1. First, see if there’s a move the computer can make that will win the game. If there is, take that move. Otherwise, go to step 2.

2. See if there’s a move the player can make that will cause the computer to lose the game. If there is, move there to block the player. Otherwise, go to step 3.

3. Check if any of the corner spaces (spaces 1, 3, 7, or 9) are free. If so, move there. If no corner piece is free, then go to step 4.

4. Check if the center is free. If so, move there. If it isn’t, then go to step 5.

5. Move on any of the side pieces (spaces 2, 4, 6, or 8). There are no more steps because if the execution reaches step 5 the side spaces are the only spaces left.

### Minimax Implementation(Alpha-Beta) has the following rules:

1. Minimax is a kind of backtracking algorithm that is used in decision making and game theory to find the optimal move for a player, assuming that your opponent also plays optimally. It is widely used in two player turn-based games such as Tic-Tac-Toe, Backgammon, Mancala, Chess, etc.

2. In Minimax the two players are called maximizer and minimizer. The maximizer tries to get the highest score possible while the minimizer tries to do the opposite and get the lowest score possible.

3. Every board state has a value associated with it. In a given state if the maximizer has upper hand then, the score of the board will tend to be some positive value. If the minimizer has the upper hand in that board state then it will tend to be some negative value. The values of the board are calculated by some heuristics which are unique for every type of game.

4. See this [article](https://www.geeksforgeeks.org/minimax-algorithm-in-game-theory-set-4-alpha-beta-pruning/) for a detailed explanation.

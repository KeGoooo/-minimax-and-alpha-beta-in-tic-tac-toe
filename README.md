# Tic-tac-toe using minimax and alpha-beta algorithms

## Introduction: 
#### In this project, we will study and understand adversarial search; we chose tic-tac-toe, and we're going to implement Mini-Max and Alpha-Beta pruning algorithms. The main idea of these algorithms is that the player wants to maximize his performance while trying to minimize his opponent's. So the algorithms are supposed to find the best move for the player..

## Adversarial search : 
#### Adversarial search: is a search in which we look at the issues that occur when we try to plan ahead in order to win, but there are opponents who plan against us in order to make sure we lose. From this, we can conclude that we are dealing with a multi-agent environment, which can be cooperative or competitive, but it's competitive in tic-tac-toe.

Tic-Tac-Toe:
Is a game in which two players switch turns after each player makes a move. The way to win is either by making a row, a column, or a diagonal of three X's or three O's.
The game can be drawn if no player has been able to make a row, a column, or a diagonal and the board has become full.
Initial state : the game initially starts with an empty board.
State space: Set of all possible remaining states
Goal state: The game ends with one player winning or a tie between them. Therefore, terminal states are win, lose, or tie.

## Mini-Max algorithm:
#### Is an algorithm used especially for games, and it is a recursive algorithm to choose the next move for the player while one player tries to choose a move with the maximum score, and the other player chooses a move with the minimum score. The main idea of the algorithm is to make a desicion to provide the optimal move from the available options assuming that the other player is also choosing the optimal options. The problem is that it has a large time complexity and it O(b^m).


## Alpha-beta pruning algorithm:
#### is the better version of the minimax algorithm, it seeks to decrease the number of nodes that are evaluated by the minimax algorithm in its search. While they both determine the optimal move for the player. However, the alpha-beta pruning will improve the time complexity by using a technique that doesn't have checking all the nodes, this technique called: pruning which allows us to compute the proper minimax choice without inspecting each node of the game tree. And we do the alpha-cut if Alpha >= Beta, also the Beta-cut happens when Beta <= Alpha.

#### Alpha-beta pruning may be done at any level in a tree, and it can occasionally trim the entire sub-tree and the tree leaves. Also, the time complexity is O(b^m/2) if the nodes are in order, and it can reach O(b^m) if there is no pruning.


## Experimental results
#### We conclude that we can't win against the computer in both algorithms but sometimes we Tie, they both will give the optimal moves but there are some obvious differences. Firstly there are some differences between mini-max and alpha-beta in time and size of tree. The alpha-beta is better ,Secondly there is a huge difference if we play first or the computer.
#### In the end alpha-beta is better in performance and less time then mini-max

# References 
1:https://medium.com/byte-tales/the-classic-tic-tac-toe-game-in-python-3-1427c68b8874

2:https://stackoverflow.com/questions/1557571/how-do-i-get-time-of-a-python-programs-execution

3:https://www.whitman.edu/documents/Academics/Mathematics/2019/Felstiner-Guichard.pdf

4:https://en.wikipedia.org/wiki/Tic-tac-toe

5:https://materiaalit.github.io/intro-to-ai/part2/

6:https://imisu-cs340.github.io/ar.html

7:Russell and Norvig, Articial Intelligence:A Modern Approach, 3rd Ed,2009.

8:David L. Poole et al, Artificial Intelligence:foundations of computational Agents,2010

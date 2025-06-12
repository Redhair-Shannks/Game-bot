

## MINIMAX Algorithm - 
* Minimax is a kind of **backtracking** algorithm.
* It is widely used in two player turn-based games such as Tic-Tac-Toe, Backgammon, Mancala, Chess, etc.
* In Minimax the two players are called **maximizer** and **minimizer**. The maximizer tries to get the highest score possible while the minimizer tries to do the opposite and get the lowest score possible.
* Time Complexity: **O(b^d)**,  Space Complexity: **O(b*d)**; where b is the branching factor and d is the maximum depth of the tree.
* **Branching Factor -** It is the number of children that each node has.

* **Limitations of Minimax algorithm -**
  *  Because of the huge branching factor, the process of reaching the goal is **slower**.
  *  Evaluation and search of all possible nodes and branches degrades the performance and efficiency of the engine.
  *  oth the players have too many choices to decide from.
  *  If there is a restriction of time and space, it is not possible to explore the entire tree.
 
* The limitation of the minimax algorithm can be improved from **alpha-beta pruning**.

## ALPHA BETA Pruning -
* Alpha-beta pruning is a modified version of the minimax algorithm. It is an optimization technique for the minimax algorithm.
*  It reduces the computation time by a huge factor (averagely upto 25%) .
*  **Alpha:** The best (highest-value) choice we have found so far at any point along the path of Maximizer. The initial value of alpha is -∞.
*  **Beta:** The best (lowest-value) choice we have found so far at any point along the path of Minimizer. The initial value of beta is +∞.
*  **Condition for Alpha-beta pruning(When we prune the tree?):** α>=β
*  The Max player will only update the value of alpha and the Min player will only update the value of beta.
*  In case of Ideal pruning, time complexity become O(b^(m/2)) [earlier it was O(b^m)].

## Heuristic Algorithm - 
* To produce a working solution within a reasonable time frame.
* Instead of looking for a perfect solution, heuristic strategies look for a **quick** solution that falls within an acceptable range of accuracy.


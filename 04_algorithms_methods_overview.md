# Problem 4

List all algorithms and methods that we have covered in this course. Write 3 sentences to describe what each algorithm and method solves etc.


- **Breadth First Search**: This algorithm works to find the shortest path to an item, location, or goal state. It does so my searching breadth wise, exploring all neighbor nodes before searching deeper. We used this in our Pacman AI algorithm for eating all the pellets in a maze.

- **Depth First Search**: This algorithm also works to find the shortest path to an item. However, unlike in DFS, it search as deep as it can first before searching neighbor nodes. We used this in our Pacman AI algorithm for eating all the pellets in a maze.

- **Uniform Cost Search**: This algorithm also works to find the shortest path to an item. It is very similar to Dijsktra's algorthm and searches using a priority queue. This priority queue is used to decide which path to take, without the use of heuristics. 

- **A\* Search**: This algorithm also works to find the shortest path to an item. However, unlike the algorithms above, A* uses a heuristic, along with the actual path cost, to determine which path to take. The heuristic used should ideally be both admissable and consistent. Admissable being that it doesn't overestimate the goal cost, and consistent being that the hueristic can at most drop a cost c when taking an action, where c is the cost of the taken action. 

- **Minimax**: Minimax is used to decide the actions to take to best maximize the reward and minimize the potential loss. The algorithm works by alternating agency between the player and the opponent. The values are calculated for the worst possible scenario, where the opponent makes the best moves possible.

- **Alpha-Beta Pruning**: This algorithm is used to prune the results given my Minimax, to make it more efficient. Instead of continiuing to evaluate a minimax tree branch, it will stop whenever a better action is found, as these lesser branches will not affect the final decision. It uses two values, alpha and beta, which represent the minumum score for the player and the maximum score for the opponent respectively. A branch is not explored whenever beta is less than or equal to alpha, as these actions will not be considered for the final result.

- **Expectimax**: Expectimax is similar to Minimax, except that it no longer assumes we are playing against a perfect opponent. Instead it uses probabilistic modeling to emulate opponent behavior, where they may not always choose the optimal action. This allows us to choose the best probability model for the opponent.

- **Value Iteration**: Value iteration is a planner which computes a Markov Decision Process (MDP) policy through backwards induction. This optimal computed policy is derived through an iterative process that runs until convergence. 

- **Q-Learning**: This algorithm is used to find a policy that will indicate which action to take under different circumstances. It takes into account the old Q value, the learning rate, and the learned value which is composed of the reward, discount factor, and estimate of the next optimal Q value. The end result allows an agent to take the best possible action given a specific state.

- **Cross-Entropy Method**: This method is used to produce better samples given a distribution that is different from the one we are interested in. It works by reducing the amount of cross entropy, which is used as a quantitave measure of the difference between two distributions, from the given distribution and the target distribition. This can be particularly helful for simulating rare-events.

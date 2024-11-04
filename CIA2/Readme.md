Reinforcement Learning on a 100x100 Grid with Obstacles
This project implements a Reinforcement Learning (RL) agent for navigating a 100x100 grid with obstacles, from a start to a goal point. The agent leverages Markov Decision Processes (MDP) and benchmarks the performance of Dynamic Programming (DP) methods against other RL algorithms.

Project Overview
Environment Setup:

A 100x100 grid environment is generated, where 20% of cells are obstacles.
Random start and goal points are assigned, ensuring they don’t overlap with obstacles.
Obstacles are marked with a value of -1 in the grid.
MDP and RL Agent:

State Space: Each cell in the grid represents a unique state.
Action Space: The agent can move up, down, left, or right.
Reward Function:
Goal state: +100.
Obstacles: -100.
Regular moves: -1.
Transition Function: Defines how the agent moves between states and avoids obstacles.

Solution Methods:

Dynamic Programming (Value Iteration):
Calculates the optimal policy and value function over the grid until convergence.

Benchmarking with Other RL Methods:
The DP-based solution is compared against other RL algorithms like Q-learning and SARSA to evaluate performance metrics (e.g., convergence rate and optimality).

Results
The agent optimizes its policy and actions to reach the goal efficiently, avoiding obstacles. The performance of DP and other RL methods can be visualized through value plots and convergence metrics.
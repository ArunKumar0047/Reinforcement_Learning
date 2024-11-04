# Hybrid ACO-RL Algorithm for Traveling Salesman Problem
This implementation combines Ant Colony Optimization (ACO) with Reinforcement Learning (RL) to solve the Traveling Salesman Problem (TSP). The hybrid approach enhances the traditional ACO algorithm by incorporating Q-learning to optimize path selection and parameter updates.


## Algorithm Overview
The algorithm combines two key approaches:

**Ant Colony Optimization (ACO)**: Uses pheromone trails and heuristic information to guide ants in constructing solutions
**Reinforcement Learning (RL)**: Employs Q-learning to optimize decision-making and enhance the exploration-exploitation balance


## Key Features
- Hybrid pheromone update mechanism incorporating Q-values
- Epsilon-greedy exploration strategy
- Dynamic parameter adjustment through Q-learning
- Eligibility traces for temporal credit assignment
- Convergence history tracking and visualization

## Implementation Details
### Parameters
- `num_ants`: Number of ants in the colony
-  `num_iterations`: Maximum number of iterations
- `alpha`: Pheromone importance factor
- `beta`: Heuristic information importance factor
- `evaporation_rate`: Pheromone evaporation coefficient
- `q_factor`: Pheromone deposit factor
- `learning_rate`: Q-learning rate
- `discount_factor`: Q-learning discount factor
- `epsilon`: Exploration probability for epsilon-greedy strategy

## Key Components

### State Selection:
Combines pheromone levels with Q-values
Uses epsilon-greedy strategy for exploration
Normalizes probabilities for next city selection


### Q-Learning Integration:
Updates Q-values based on route quality
Uses TD-error for value function approximation
Incorporates eligibility traces


### Pheromone Update:
Combines traditional ACO pheromone update with Q-table information
Implements evaporation and deposit mechanisms
Ensures bounded pheromone levels

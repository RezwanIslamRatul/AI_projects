This Python code presents an implementation of a grid-based pathfinding algorithm with battery management using A* and UCS (Uniform Cost Search). 

PriorityQueue Class:
Implements a priority queue to order elements based on their priority.
Used in the A* and UCS algorithms to manage nodes during the search.

Node Class:
Represents a state in the search tree.
Contains information about the state, parent, action, and path cost.
Implements a comparison operator for the priority queue.

Environment Class:
Represents the grid layout, starting position, and goal position.
Defines actions, result, and goal-checking functions for the agent.

Agent Class:
Manages the agent's interaction with the environment.
Implements A* and UCS search algorithms with battery management.
The battery depletes with each action, and the agent recharges when it reaches 0%.

Visualization Function:
Plots the grid, start, goal, and the found path using matplotlib.

Random Grid Generation Function:
Generates a random grid with obstacles based on the specified size and obstacle probability.

Execution:
A random grid is generated with a specified size and obstacle probability.
An agent is created with an initial battery level(100).
A* search with battery management and UCS search with battery management are executed.
The solution paths and visualizations are printed for both algorithms.

Changes from the given code:

Battery Management: The a_star_search_with_battery and ucs_search_with_battery methods now include battery management. 
After each action, the battery level is decreased by 10 units. If the battery level  0, it's recharged to 100%

Initialization: The __init__ method now takes  the env parameter and battery parameter which is initialized to 0 .
 The battery level is initialized within each search method (a_star_search_with_battery and ucs_search_with_battery)

Uniformed search function:
A function named ucs_search_with_battery is added to perform the ucs search.

Print Functionality: The print_current_state_with_battery method is added 
to print the current state and battery level during the search process.

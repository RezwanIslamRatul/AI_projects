1. Approaches

This assignment implemented a genetic algorithm (GA) to solve a task assignment problem. The goal was to assign tasks to robots while considering:

Task characteristics: Duration and priority.
Robot capabilities: Efficiency in completing tasks.
The GA aimed to find an optimal assignment that minimizes the total completion time and workload imbalance while prioritizing high-priority tasks.

2. Implementation Details

The code utilizes several key components:

Data Generation: The generate_mock_data function creates random data for tasks (duration, priority) and robots (efficiency).
Genetic Algorithm:
Population: A collection of candidate solutions (task assignments) represented as integer arrays.
Fitness Function: calculate_fitness evaluates a solution based on total completion time, workload balance, and weighted task priority. Higher fitness signifies a better solution.
Selection: tournament_selection chooses parents for reproduction based on a competition between a small group of individuals.
Crossover: single_point_crossover combines genetic material from two parents to create offspring solutions.
Mutation: task_swapping_mutation introduces random changes by swapping tasks within a solution.
Visualization: visualize_assignments_improved displays the final task assignment as a heatmap with task durations, priorities, and robot efficiencies.
3. Challenges Faced
 The fitness function combines multiple objectives (completion time, workload balance, priority). Tuning the weights for these objectives were challenging to achieve the desired balance .
5. How GA Helps Optimize Task Assignments

GAs offer several advantages for this task assignment:

GA  handled problems with complex constraints and varying task/robot characteristics.It explored a diverse set of solutions simultaneously and increased the chance of finding good solutions even in large search spaces.It has also given the continueous improvement.

6. Implications of Findings
Reduced Completion Time: Tasks are completed faster by assigning them to the most suitable robots.
Improved Workload Balance: Workload is evenly distributed among robots, preventing underutilization or overloading.
Enhanced Efficiency: Prioritizing high-importance tasks ensures that critical tasks are completed first.

Overall this genetic algorithm approach can be further improved for more complex real-world task assignment problems.

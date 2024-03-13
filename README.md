# EvoMaze-Explorer
# Evolutionary Path Finding in Mazes

This project implements an evolutionary algorithm to find optimal paths through mazes using Python. The algorithm evolves a population of candidate paths, selecting and reproducing the fittest individuals (shortest paths) through genetic operations like mutation and crossover.

## Features

- Generation of random mazes using the `python-maze` library
- Representation of paths as sequences of moves (up, down, left, right)
- Fitness evaluation based on path length and ability to reach the maze exit
- Tournament selection for parent selection
- Mutation and crossover operators for generating new offspring paths
- Elitism to preserve the fittest individuals across generations
- Niching to maintain diversity in the population
- Adaptive mutation rate for better exploration and exploitation balance

## Usage

1. Install the required dependencies: `pip install python-maze`
2. Run the `main.py` script, which will:
   - Generate a random maze
   - Initialize a population of random paths
   - Evolve the population over multiple generations
   - Visualize the best paths found every 10 generations
   - Display the final, fittest path through the maze

## Results

After running the evolutionary algorithm, the best path found is visualized on the console by marking it with 'o' characters on the maze grid. The algorithm effectively finds short paths through the maze, and the adaptive parameters help balance exploration and exploitation for better convergence.

## Future Improvements

- Experiment with different genetic representations (e.g., path segments, decision trees)
- Implement alternative selection methods (e.g., roulette wheel, rank-based)
- Explore other genetic operators (e.g., inversion, edge recombination)
- Incorporate domain-specific heuristics or guidance for path finding
- Parallelize the fitness evaluation and evolutionary process
- Extend the algorithm to 3D mazes or more complex environments

Feel free to modify the code, experiment with different parameters, and contribute your improvements!

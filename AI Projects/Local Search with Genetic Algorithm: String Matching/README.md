# Local Search with Genetic Algorithm: String Matching
In this assignment, I implemented a Genetic Algorithm (GA) to solve a string matching problem by evolving candidate solutions toward a target string. The task was framed as an optimization problem, where the goal is to minimize the difference between a candidate string (phenotype) and a known target string.

Each individual in the population is encoded as a list of characters (genotype), and evaluated using an objective function that computes the character-wise difference from the target string. This minimization objective was converted into a fitness function for the GA, where higher fitness indicates a closer match.

The algorithm was configured with standard evolutionary operations:

Crossover to recombine parent genotypes

Mutation to introduce random variation

Selection using either roulette wheel or tournament selection strategies

Key hyperparameters like population size, number of generations, crossover rate, and mutation rate were tunable. Every 10 generations, the best candidate's fitness, genotype, and phenotype were printed to visualize progress. The algorithm returned the best individual found after all generations.

This problem provided an engaging way to visualize how a GA can converge on an optimal solution through iterative improvement over a search space.
# Solving Normal Form Games with Successive Elimination of Dominated Strategies (SEDS)
In this assignment, I implemented a solver for Normal Form Games using the Successive Elimination of Dominated Strategies (SEDS) method to identify pure strategy Nash equilibria. The solver supports both strong and weak dominance elimination, allowing flexible exploration of game theory strategy profiles.

The function accepts a 2D payoff matrix representing a two-player game and iteratively eliminates dominated rows (strategies for Player 1) and columns (strategies for Player 2) based on whether they are strictly or weakly dominated. The process continues until no further eliminations are possible.

Key features:

Accepts any rectangular matrix of tuple payoffs (e.g., (P1 payoff, P2 payoff))

Handles both strict and weak dominance via a weak=True flag

Returns the strategy indices of the remaining equilibrium strategy profile, or an empty list if no pure strategy Nash equilibrium is found

This implementation models how rational agents can reduce strategic complexity in competitive environments by iteratively removing clearly inferior options.


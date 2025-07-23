# Constraint Satisfaction Problem: Map Coloring
In this assignment, I implemented a Constraint Satisfaction Problem (CSP) solver to address the Map Coloring problem based on the Four Color Theorem, which states that any planar map can be colored using at most four colors such that no adjacent regions share the same color.

The map is represented as a graph-based dictionary with:

nodes: an ordered list of region names (e.g., counties or countries),

edges: a list of tuples indicating adjacency between regions (based on node indices),

coordinates: abstract drawing coordinates for use with NetworkX visualizations.

The solver uses a recursive backtracking algorithm to assign valid colors to each node while satisfying all constraints:

No two adjacent nodes can share the same color.

A valid coloring uses a predefined number of colors (typically 3 or 4).

Key components of this assignment:

Recursive CSP backtracking search

Use of deepcopy to avoid entangled state between recursive calls

Optional visualization using NetworkX and matplotlib

Tested on example maps like Connecticut and Europe

This problem demonstrates how AI techniques like CSPs can be applied to solve classic graph coloring problems with real-world geographic data.


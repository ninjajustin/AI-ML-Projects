# Forward Planner (AI Planning)
Implemented a forward state-space planner that generates a sequence of grounded actions to reach a goal state from an initial world state. Used graph search and unification to match action preconditions with the current state. Designed a recursive unification mechanism to support multiple valid bindings and ensure all applicable actions were explored.

Parsed STRIPS-like actions and states expressed in s-expressions

Applied DFS-based graph search to explore possible plans

Handled multiple unification paths and backtracking for correctness

Returned a plan (action sequence) or full execution trace (if intermediate=True)

Goal: Automatically generate a plan using available actions and initial facts to reach a desired goal state.


# Reinforcement Learning in the Game of Nim
This assignment focuses on applying Q-learning, a reinforcement learning (RL) method, to the classic combinatorial game of Nim. The objective was to develop an agent that learns to play optimally through self-play and reinforcement feedback, and to enhance its strategy using improved reward shaping.

Main Concepts & Tasks:
Environment: The Nim game with 3 piles of up to 10 items each, where players alternate removing items from piles.

Agents: The Q-learning player (learner), random player, and the rule-based Guru player. The Guru is also considered an agent, though not learned-based.

States: The full state space includes all combinations of pile counts: 11 × 11 × 11 = 1,331 possible states.

Actions: On the first move, player 1 can make 30 unique actions (i.e., choosing 1–10 items from each of 3 piles).

Rewards: Wins yield positive rewards, while losses are penalized to encourage better strategies over time.

Key Improvements:
Enhanced the Q-learning agent by introducing a loss penalty during Q-table updates, improving convergence.

Trained the improved agent against both the Random player and the Guru to collect better experience.

Demonstrated performance gains over the baseline implementation by evaluating win rates against both opponents.

This project highlights the application of RL techniques in discrete, strategic environments and emphasizes the importance of thoughtful reward design in accelerating agent learning.
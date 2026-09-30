# Pacman MDP Agent (Value Iteration)

> A planning agent that models the Pacman board as a Markov Decision Process and uses value iteration to choose safe, high-value routes.

🔒 **The source code is in a private repository** because this was university coursework at King's College London. I'm happy to walk through the code on request.

## Overview
Rather than reacting greedily one step at a time, this agent plans ahead across the whole board. Each game state is converted into a grid-based utility map, value iteration runs until the utilities converge, and Pacman then moves towards the highest-utility neighbouring cell. The agent was built to win consistently on both small and medium layouts.

## What I built
- **Reward map:** positive rewards for food and capsules, negative rewards for danger zones around ghosts
- **Adaptive behaviour:** when ghosts become edible, Pacman switches to chasing them instead of only avoiding them
- **Value iteration:** Bellman updates over the traversable grid with a tunable discount factor and convergence threshold
- **Action selection:** chooses among legal moves by expected utility

## Skills demonstrated
Markov Decision Processes · dynamic programming · planning under uncertainty · reward shaping

## Tech stack
Python

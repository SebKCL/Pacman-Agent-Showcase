# Pacman MDP Agent (Value Iteration)

> My agent treats the Pacman board as a Markov Decision Process and plans safe, high-value routes with value iteration.

🔒 The code sits in a private repository because this was King's College London coursework. Ask me and I'll walk you through it.

## Overview
The agent plans across the whole board on each turn. It builds a utility map of the grid, runs value iteration until the values settle, then steps to the neighbouring cell with the highest utility. I tuned it to win on small and medium layouts.

## What I built
- **Reward map:** food and capsules score positive, and the cells around ghosts score negative
- **Ghost hunting:** once ghosts turn edible, Pacman chases them
- **Value iteration:** Bellman updates over every open cell, with a tunable discount factor and stopping threshold
- **Move choice:** Pacman picks the legal move with the highest expected utility

## Skills
Markov Decision Processes · dynamic programming · planning under uncertainty · reward shaping

## Tech stack
Python

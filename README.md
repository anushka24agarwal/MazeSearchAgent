# Maze Search Agent

## Overview

This project implements a search agent for robotic path planning in a maze environment. The goal is to compare multiple search algorithms and evaluate their performances in finding the optimal path from a start position to a goal.

## Algorithms Implemented

1. BFS (Breadth-First Search) – Explores all nodes at the present depth level before moving to the next level.

2. DFS (Depth-First Search) – Explores as far as possible along each branch before backtracking.

3. A* (A-Star Search) – Uses a heuristic function to prioritize paths leading to the goal efficiently.

4. IDA* (Iterative Deepening A-Star Search) – Combines depth-first search with A*'s heuristic to limit memory usage while ensuring optimality.

## How It Works

1. Maze Representation - The maze is represented as a grid with walls, open paths, start, and goal positions.

2. Algorithm Selection - The user selects one of the four search algorithms to execute.

3. Pathfinding Execution - The selected algorithm explores the maze and finds the shortest or most efficient path to the goal.

4. Performance Evaluation - The number of explored nodes and execution time are recorded to compare algorithm efficiency.

## Run

Some execution commands are shown below:

```bash
python3 maze.py -m arena1.txt -bfs
python3 maze.py -m arena2.txt -dfs -astar -ida
python3 maze.py -m arena3.txt -all

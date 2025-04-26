
# A* Pathfinding Algorithm

This is a visualization of the **A* (A-Star) Pathfinding Algorithm** using **Python** and **Pygame**. The algorithm is used to find the shortest path from a start point to an endpoint on a grid while avoiding obstacles (barriers). The program allows the user to interact with the grid, place the start, end, and barriers, and visualize how the A* algorithm computes the shortest path.

## Features

- **Start and End Points:** The user can set the start and end points on the grid.
- **Obstacles:** The user can place obstacles (barriers) on the grid that the pathfinding algorithm must avoid.
- **A* Algorithm Visualization:** The algorithm computes the shortest path from the start to the end, navigating around obstacles.
- **Real-time Visualization:** The grid updates in real-time, showing the open and closed nodes, the current path, and the final solution.

## Requirements

To run this project, you need to have the following installed on your system:

- **Python 3.x**
- **Pygame**: Used for graphical rendering and interaction.

### Install Pygame

You can install Pygame using `pip`:

```bash
pip install pygame
```

## How to Run

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/tokhirasulov/SnakeGame.git
   ```

2. Navigate to the project directory:

   ```bash
   cd AStar
   ```

3. Run the Python script:

   ```bash
   python main.py
   ```

## Controls

- **Left Click**: Click to set the **start**, **end**, or **place barriers** on the grid.
- **Right Click**: Right-click to **reset** any selected nodes (start, end, or barrier).
- **Spacebar**: Press the spacebar to run the **A* algorithm** and find the shortest path.
- **C**: Press the "C" key to **clear** the grid and start over.

## Algorithm

The A* algorithm finds the shortest path by combining the advantages of **Dijkstra's Algorithm** and **Greedy Best-First-Search**. It uses a heuristic function to estimate the cost of the cheapest path from the current node to the goal, while also considering the cost of the path from the start node to the current node.

The algorithm maintains a set of open nodes (nodes to be evaluated) and a set of closed nodes (nodes that have already been evaluated). The open set is ordered by the estimated total cost, and the algorithm expands nodes with the lowest cost first.


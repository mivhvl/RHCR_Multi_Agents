# **Lifelong Multi-Agent Pathfinding (MAPF) Solver: Recreating RHCR Experiment**

This project recreates the experiments presented in the paper **"Rolling-Horizon Collision Resolution for Multi-Agent Pathfinding"** (arXiv:2005.07371). The authors propose **Rolling-Horizon Collision Reduction (RHCR)** to solve the lifelong MAPF problem, aiming to maximize throughput while avoiding collisions.

The experiment decomposes lifelong MAPF into a sequence of windowed MAPF instances and replans paths every h timesteps, interleaving planning and execution.

## Features

- Implements RHCR using:
	- **Conflict-Based Search (CBS)**
	- **Enhanced Conflict-Based Search (ECBS)**
	- **Cooperative A***
	- **Priority-Based Search**
- Two types of simulations:
	- 
- Compares **RHCR** to:
	- Holding Endpoints
	- Reserving Dummy Paths
- Outputs metrics for:
	- Throughput: Total tasks completed.
	- Runtime: Execution time of the algorithms.

## Files in the Repository

- `NOTEBOOK.ipynb`: Jupyter Notebook containing all simulations and analyses.
- `RESULTS.xlsx`: Excel file summarizing throughput and runtime results.

## User-Defined Parameters

- **Time Horizon (`w`):** Determines the window size for planning.
- **Replanning Period (`h`):** Number of timesteps between replanning events.

## Key Results

- **Throughput:** Comparable to the results reported in the paper.
- **Runtime:** Significantly smaller in our tests, likely due to improved computational resources.

## References

This implementation is based on the following paper and repository:

- Jiaoyang Li, Andrew Tinka, Scott Kiesel, Joseph W. Durham, T. K. Satish Kumar and Sven Koenig. Lifelong Multi-Agent Path Finding in Large-Scale Warehouses (extended abstract). In Proceedings of the International Joint Conference on Autonomous Agents and MultiAgent Systems (AAMAS), pages 1898-1900, 2020. (arXiv:2005.07371).
- https://github.com/Jiaoyang-Li/RHCR/tree/master

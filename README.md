# Vehicle Routing Problem With Stochastic Demands (VRPSD)

This repository contains the files and project report for the Research Practice I course, focusing on the Vehicle Routing Problem with Stochastic Demands (VRPSD). The project was carried out by Juan José Castrillón and Juan Carlos Rivera and is presented in a detailed format with the following structure:

## Repository Contents

1. **PDF Report**:
    - `Presentacion_PI1.pdf`: Detailed document including the introduction, problem definition, methodology, results, and conclusions.

2. **Source Code**:
    - `vrpsd_grasp`: Implementation of the GRASP (Greedy Randomized Adaptive Search Procedure) algorithm.
    - `split_s`: Split-S procedure for the TSP problem.
    - `gurobi_partition`: Set partitioning using Gurobi.
    - `capacity_simulation`: Simulation of vehicle capacity constraints.

## Project Description

### Introduction

The goal of the project is to optimize vehicle routes under uncertain customer demands. A comprehensive algorithm was implemented in Python, integrating advanced techniques such as GRASP, Split-S, and a partitioning model with Gurobi.

### Problem Definition

The problem addresses a complete undirected graph \(G = (V, E)\), where \(V = \{0, 1, ..., n\}\) represents the nodes and \(E\) the edges. Each customer \(i \in V \setminus \{0\}\) has a stochastic demand \(\xi_i\), and vehicles have a capacity \(Q\). The objective is to minimize the expected total cost, including travel and overload costs, while considering recharge actions such as returning to the depot or receiving assistance from another vehicle.

### Methodology

The methodology consists of the following phases:

1. **GRASP Heuristic Algorithm**: Construction of an initial solution and improvement through local search.
2. **Split-S Procedure for TSP**: Division of the TSP solution into sub-routes based on the number of available vehicles.
3. **Set Partitioning with Gurobi**: Optimization of route combinations to minimize the total distance traveled.
4. **Capacity Constraint Simulation**: Simulation of demands using a normal distribution and evaluation of two approaches: return to the depot and assistance from nearby vehicles.

### Results

- **Instance 1**: Graphical comparison of routes and total distances traveled under different simulations.
- **Summary Table**: Summary of the total distances traveled across three instances, highlighting the efficiency of the implemented approaches.

### Conclusions and Future Research

- Parallel simulation significantly improves solutions.
- Assistance from nearby vehicles reduces the total distance traveled.
- Important contributions to route optimization under stochastic demands.
- Proposals for future research include analyzing the impact of different demand distributions and applying machine learning techniques.

## References

1. Magdalene Marinaki, Andromachi Taxidou, and Yannis Marinakis. “A hybrid Dragonfly algorithm for the vehicle routing problem with stochastic demands”. In: Intelligent Systems with Applications 18 (2023), p. 200225. doi: [https://doi.org/10.1016/j.iswa.2023.200225](https://doi.org/10.1016/j.iswa.2023.200225).
2. Jorge E. Mendoza and Juan G. Villegas. “A multi-space sampling heuristic for the vehicle routing problem with stochastic demands”. In: Optimization Letters 7 (2013). doi: [https://link.springer.com/article/10.1007/s11590-012-0555-8](https://link.springer.com/article/10.1007/s11590-012-0555-8).
3. Majid Salavati-Khoshghalb et al. “A hybrid recourse policy for the vehicle routing problem with stochastic demands”. In: EURO Journal on Transportation and Logistics 8.3 (2019), pp. 269–298. doi: [https://doi.org/10.1007/s13676-018-0126-y](https://doi.org/10.1007/s13676-018-0126-y).

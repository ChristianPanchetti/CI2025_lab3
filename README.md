# Shortest Path Algorithms 

This repository contains a complete solution for **Lab 3** on shortest–path algorithms.

The goals are:

1. Generate random instances of a **directed weighted graph** where nodes represent cities.
2. Compute the **shortest path between all pairs of cities**.
3. Implement our own versions of:
   - Dijkstra
   - Bellman–Ford
   - A\* (with Euclidean heuristic)
4. Compare our implementations with the corresponding **NetworkX** algorithms.
5. Print **global statistics** and check whether the results match.

---

## 1. Project structure

- `Shortest_Path_Algorithms.ipynb`  
  Main script. It:
  - builds random problem instances
  - runs all–pairs shortest paths
  - compares our algorithms with NetworkX
  - prints global statistics

There is no separate module file on purpose to keep the lab easy to inspect.

---

## 2. Problem generation

The function:

```python
generate_problem(
    n_nodes: int,
    edge_density: float,
    allow_negative: bool,
    noise_amplitude: float,
    seed: int = 42,
) -> ProblemInstance
```

---
Made with Simone Ventura, github: https://github.com/gambatz.

Portions of the algorithmic optimization were refined with the assistance of ChatGPT.
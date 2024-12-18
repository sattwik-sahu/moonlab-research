---
tags:
  - resources/reading
---

> [!tldr] TLDR;
> Graph cuts segment graphs into disjoint subsets of vertices based on criteria on the edges between vertices.
> 
> They are used extensively in image segmentation tasks, involving figure-ground-segregation, interactive segmentation, etc.

# Terminology

Assume a graph $G$ with vertices $V = \{v_1, v_2, \dots \}$ and edges $E = \{e_1, e_2, \dots\},\ e_i \in V \times V$

## Cut

A subgraph $G' \in G$ separated using the graph cut algorithm.

## Minimum Cut

The cut with the lowest weight among all possible cuts in the graph. Helps in determining the way to segment the graph $G$ into cuts with lowest cost.

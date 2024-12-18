---
tags:
  - resources/reading
---
> [!tldr] TLDR;
> - Superpixels represent a method of *grouping pixels* into *perceptually meaningful regions*.
> - Superpixels are **clusters of pixels** that share *similar color and texture characteristics*, effectively forming regions that *align better with the boundaries* of objects within an image.

---

# Why?

1. **Discretization**: Pixels are merely a result of discretizing continuous images, which can lead to inefficiencies.
2. **Computational Feasibility**: Large images with hundreds of thousands of pixels can overwhelm many algorithms, making them computationally infeasible.

# How?

1. **SLIC (Simple Linear Iterative Clustering)**: This widely used algorithm clusters pixels based on their color and spatial proximity, producing superpixels that are compact and adhere closely to object boundaries.
2. **Graph-based methods**: These approaches treat pixels as nodes in a graph, where edges represent affinities based on color similarity. The segmentation is then achieved by partitioning the graph to minimize an error objective

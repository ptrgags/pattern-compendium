---
layout: article
thumbnail: spanning-tree-grid.png
thumbnail_alt: A square grid with lines connecting all 8x8 squares together into a tree.
title: Spanning Tree (Rectangular Grid)
---

## Definition

**Building Blocks**

- A rectangular grid where all cells are initially disconnected from each other

**Rules**

- Each individual grid cell is a **connected component**
- Select two connected components $A$ and $B$ that meet the following criteria:
    - They must not share any grid cells
    - There must be at least one pair of cells $a \in A, b \in B$ where $a, b$
    are adjacent either horizontally or vertically
    - There must not be any edges between $A$ and $B$
- Connect one of the pairs of adjacent cells $a, b$. Now $A$, $B$, and the new edge form a connected component.
- Continue connecting pairs of connected components until the whole grid is a single connected component. This is a **spanning tree**

## Related Patterns

This pattern is a special case of [Spanning Tree](./spanning-tree). Adding
a rectangular grid restricts the placement of vertices and edges.

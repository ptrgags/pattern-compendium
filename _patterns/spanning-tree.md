---
layout: article
thumbmnail: spanning-tree.png
thumbnail_alt: A collection of points connected by lines. All points are connected, and there are no cycles.
title: Spanning Tree
---

## Definition

**Building Blocks**

- A number of disjoint vertices

**Rules**

- A single vertex is defined to be **connected component**
- Take two connected components $A, B$ that do not share any vertices or edges. Add a single edge between a vertex from $A$ and a vertex from $B$. The combination of $A$, $B$ and the new edge is a connected component
- Continue combining connected components until all vertices are part of a single large connected component. This is called a **spanning tree**


## Related Pattern

- This pattern is a more general case of [Spanning Tree (Rectangle Grid)](./spanning-tree-grid)

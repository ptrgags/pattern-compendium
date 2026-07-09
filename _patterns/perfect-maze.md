---
layout: article
thumbnail: perfect-maze.png
thumbnail_alt: A diagram of a maze
title: Perfect Maze
---

## Definition

**Building Blocks**

- a rectangular grid

**Rules**

- Compute a [Spanning Tree](./spanning-tree-grid) on the grid. This represents the connections between rooms.
- On a new grid of the same size, draw the walls of the maze:
    - For each grid cell edge that did not have a connection, draw a wall in the corresponding cell of the new grid.
    - For each grid cell edge that had a connection, leave it blank in the new grid. This is interpreted as a "hallway" between rooms.
- The end result is a **perfect maze**

## Other Notes

TODO: Add citation for _Mazes for Programmers_

---
layout: article
thumbnail: line-thumbnail.png
thumbnail_alt: 
title: Line
---

## Recipe: Straightedge and Compass

- Draw two points in the plane, A and B
- Line up a straightedge so it just touches both points
- Trace the edge of the straightedge, producing a line that cuts through
both points.

## Recipe: Normal and Distance from Origin

## Recipe: Normal and Point on Line

$$ \vec{r} \cdot \vec{n} = \vec{p}_0 \cdot \vec{n}$$

where:

- $\vec{n}$ is a normal vector, i.e. a vector that points perpendicular to the 
    line. It is often convenient to have 
- $\vec{p_0}$ is some point known to be on the line.

Note that $\vec{p}_0 \cdot \vec{n}$ is the distance from the line $d$
described in the previous section!

The above equation can be rewritten

$$ (\vec{r} - \vec{p}_0) \cdot {n} = 0$$

## Recipe: As Trajectory

A line can be traced 

$$L(t) = x_0 + vt$$

Where:

- $x_0$ is the start point 
- $v$ is the velocity
- $t$ is the time (or some other notion of "progression"). It can be any real number.

## Recipe: As Linear Extrapolation

$$L(t) = \text{lerp}(A, B, t) = (1 - t)A + tB$$

where $t \in \mathbb{R}$

## Recipe: Slope-intercept Form

This is the form you may remember from math class:

$$y = mx + b$$

where:

- $m$ is the slope of the line. 0 means horizontal. Negative values produce lines that slope downwards and to the right. Positive values produce lines that slope upwards. 
- $b$ is the y-intercept

Vertical lines cannot be represented by this form, instead use

$$x = a$$

where $a$ is the x-intercept.

## Recipes: Plane-Based Geometric Algebra

In Plane-based Geometric Algebra (PGA), there are two different ways to produce
a line

First, you can join two points into a line

$$L = A \vee B$$

## Recipe: Signed Distance Field

$$\vec{r} \cdot \vec{n} - d = 0$$

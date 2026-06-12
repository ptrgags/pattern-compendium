---
layout: default
---
# Symmetry

In math, there are a few different definitions of symmetry depending on the
context. However, all are closely related.

At a high level, a **symmetry** of an object is a transformation that leaves
it unchanged in some sense that depends on context.

## Note on Terminology

In the sections below, I use the following terminology:

- **transformation** - a function from a set to itself
    - e.g. $a: X \to X$
- **function** - for more general functions that may map between different sets
    - e.g. $f: X \to Y$
- **input transformation** - a transformation on the domain of a function
    - e.g. $a: X \to X$
- **output transformation** - a transformation on the codomain of a function
    - e.g. $b: Y \to Y$

All of these are functions, but these terms provide hints as to how they are
used in patterns.

I don't assume any further properties of these functions unless otherwise noted.

## Symmetry of a Function

Given a function $f:X \to Y$, an input transformation
$a: X \to X$, is a **symmetry of** $f$ when

$$f \circ a = f$$

Sometimes this is phrased as "$f$ is $a$-symmetric."

## Generalized Symmetry

Given a function $f: X \to Y$, an input transformation $a: X \to X$, and
an output transformation $b: Y \to Y$, $(a, b)$ is a **symmetry of** $f$
when

$$f \circ a = b \circ f$$

Sometimes this is phrased as "$f$ is $(a, b)$-symmetric"

## Fixed Points

A **fixed point** is a point $x \in X$ that stays in place when being 
transformed by a transformation $a:X \to X$

$$a(x) = x$$

Sometimes this is phrased as "$a$ fixes $x$"

## Fixed Sets

We can zoom out and look at collections of points that stay in place under
a transformation. If $S$ is a set and $a: X \to X$ is a transformation, then
$S$ is a **fixed set** whenever 

$$f(S) = \{f(x) | x \in S \} = S$$

Similar to fixed points, we can say "$a$ fixes $S$"

### Subtlety About Fixed Sets

> [!IMPORTANT]
> A set of fixed points is a fixed set, but a fixed set does not
> need to include any fixed points!

If you gather a set of fixed points and apply a transformation to the whole
set, each point will remain fixed, and therefore the set will be fixed.

<details>

<summary>Proof</summary>

Let $a: X \to X$ be a transformation and $F$ be a set of fixed points
of $a$. We want to prove that $a(F) = F$.

Expanding the left hand side, we get

$$a(F) = \{a(x) | x \in F\}$$

but each $x$ is a fixed point of $a$, so $a(x) = x$ by definition.

$$\{a(x) | x \in F\} = \{x | x \in F\} = F$$
</details>

## Identity, the Strongest Form of Symmetry

> [!IMPORTANT]
> Every function/point/set has identity symmetry

An identity transformation $I:X \to X, I(x) = x$ is a "do nothing" transformation,
it simply returns its input unchanged.

This is a very strong form of symmetry because it works on any function, point
and set you can throw at it. 

- Functions: $f \circ I = f$
- More generally: $f \circ I_X = I_Y \circ f$ (since the input and output might be different sets)
- Fixed Points: $I(x) = x$
- Fixed Sets: $I(S) = S$

## More Notes

🚧 Outline for now

- ❓ how to generalize further to functions of 2+ variables?
- I haven't explored other notions of symmetry such as symmetric relations
- This page needs some concrete examples and images
    - function symmetry... maybe a parabola?
    - a checkerboard as an image would be a good example 
- Things to cite (need to add some things to Jekyll to help manage these)
    - [Math Stack Exchange post](https://math.stackexchange.com/a/94951) about the generalized symmetry formula in 
        - ❓ that post assumes that the transformations are automorphisms... how necessary is that?
    - 📗_Creating Symmetry_ by Frank Farris - this book talks about function symmetries and generalized symmetries
    - Check 📗_Fractals Everywhere_, does it mention any of this?
    - ...blanking on the name of a symmetry book by John Conway, see if that had any relevant definitions.

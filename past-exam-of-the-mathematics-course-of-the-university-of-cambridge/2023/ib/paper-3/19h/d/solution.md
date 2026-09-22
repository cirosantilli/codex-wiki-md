<h1 id="19h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Orient every edge of the feasible [convex polytope](../../../../../../convex-polytope.md) in the direction of increasing objective. Write

$$
O=000,\qquad A=(1/2,1,1),\qquad
B=(1,1/2,1),\qquad C=(1,1,1/2).
$$

The possible improving [simplex method](../../../../../../simplex-method.md) paths from $O$ to $A$ are

$$
\begin{aligned}
&O\to010\to011\to A,
&&O\to001\to011\to A,\\
&O\to100\to110\to C\to A,
&&O\to010\to110\to C\to A,\\
&O\to100\to110\to C\to B\to A,
&&O\to010\to110\to C\to B\to A,\\
&O\to100\to101\to B\to A,
&&O\to001\to101\to B\to A.
\end{aligned}
$$

These exhaust the directed edge graph: the ordinary cube edges remain except those incident to the removed vertex $111$; each such edge ends at one of $A,B,C$; and the cutting face contributes the triangle with edges $AB,AC,BC$.

The first two paths use three pivots, while the two paths through both $C$ and $B$ use five. Therefore the smallest and largest possible numbers of simplex steps are

$$
\boxed{3\text{ and }5},
$$

and the total number of distinct outcomes is

$$
\boxed{8}.
$$

This is the [simplex paths on a cube with one truncated corner](../../../../../../simplex-paths-on-a-cube-with-one-truncated-corner.md) calculation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [19H](../../19h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

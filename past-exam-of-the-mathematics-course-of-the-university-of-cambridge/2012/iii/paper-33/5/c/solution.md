<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $L$ be the fixed line and choose $y\in L$. Take orthonormal vectors $e_1,e_2$ spanning the plane perpendicular to $L$. The process

$$
Y_t=\bigl(e_1\cdot(B_t-y),e_2\cdot(B_t-y)\bigr)
$$

is standard planar [Brownian motion](../../../../../../brownian-motion-split.md) starting from $Y_0\ne0$. Indeed the projected increments are centered [Gaussian random vectors](../../../../../../gaussian-random-vector.md) with covariance $(t-s)I_2$, are [independent](../../../../../../independent-random-variables.md) on disjoint intervals, and have continuous paths.

The event $B_t\in L$ is exactly $Y_t=0$. The [polar point for planar Brownian motion](../../../../../../polar-point-for-planar-brownian-motion.md) result in (b) therefore gives

$$
\boxed{\mathbb P_x(\exists t\geq0:B_t\in L)=0\qquad(x\notin L).}
$$

This is a [projection criterion for Brownian avoidance of affine subspaces](../../../../../../projection-criterion-for-brownian-avoidance-of-affine-subspaces.md): avoiding a fixed point in a two-dimensional projection excludes hitting the original line.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

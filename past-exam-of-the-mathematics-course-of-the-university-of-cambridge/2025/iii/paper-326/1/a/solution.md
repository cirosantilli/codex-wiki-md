<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a minimizing sequence for the [variational regularization](../../../../../../variational-regularization.md) functional

$$
F(u)=\frac12\|Au-f\|_Y^2+\alpha J(u).
$$

Its [coercivity](../../../../../../coercive-function.md) makes the sequence bounded. Since $X$ is a [reflexive Banach space](../../../../../../reflexive-banach-space.md), a subsequence converges weakly to some $u\in X$. A convex norm-lower-semicontinuous functional has [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md), so this applies to both $J$ and the convex continuous map $u\mapsto\|Au-f\|_Y^2$. Therefore

$$
F(u)\leq\liminf_nF(u_n)=\inf_XF,
$$

and $u$ is a minimizer. This is the [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

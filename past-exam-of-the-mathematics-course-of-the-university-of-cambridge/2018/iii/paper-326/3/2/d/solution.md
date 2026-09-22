<h1 id="3/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\iota_C$ for the [indicator functional of a constraint set](../../../../../../../indicator-functional-of-a-constraint-set.md) $C$ and $q(u)=\|u\|^2/2$. Then

$$
d_C=\iota_C\mathbin\square q.
$$

Both terms are [convex](../../../../../../../convex-function.md), hence their [infimal convolution](../../../../../../../infimal-convolution.md) is the [convex](../../../../../../../convex-function.md) [squared distance to a convex set](../../../../../../../squared-distance-to-a-convex-set.md). The [closest point theorem in a Hilbert space](../../../../../../../hilbert-projection-theorem.md) supplies the unique [metric projection onto a closed convex set](../../../../../../../euclidean-projection-onto-a-convex-set.md) $P_Cu$ and gives $d_C(u)=\|u-P_Cu\|^2/2$.

Identify the [Hilbert space](../../../../../../../hilbert-space-split.md) with its [dual space](../../../../../../../dual-space.md) using the [Riesz representation theorem](../../../../../../../riesz-representation-theorem.md). Completing the square yields $q^*(p)=\|p\|^2/2$, while $\iota_C^*(p)=\sup_{v\in C}\langle p,v\rangle=\sigma_C(p)$ is the [support function](../../../../../../../support-function.md). The [conjugate of the squared distance to a convex set](../../../../../../../conjugate-of-the-squared-distance-to-a-convex-set.md) is therefore

$$
\boxed{d_C^*(p)=\frac12\|p\|^2+\sigma_C(p).}
$$

For the closed unit ball, the [metric projection onto a closed convex set](../../../../../../../euclidean-projection-onto-a-convex-set.md) is $P_Cu=u$ if $\|u\|\leq1$, and $P_Cu=u/\|u\|$ otherwise. Therefore

$$
\boxed{d_C(u)=\frac12\bigl(\max\{\|u\|-1,0\}\bigr)^2,\qquad
d_C^*(p)=\frac12\|p\|^2+\|p\|.}
$$

The last equality uses the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) to compute the unit ball's [support function](../../../../../../../support-function.md), attained in the direction of $p$ when $p\neq0$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

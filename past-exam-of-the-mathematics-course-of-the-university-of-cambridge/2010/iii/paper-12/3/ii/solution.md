<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use the directed set version of the [Talagrand convex distance](../../../../../../talagrand-convex-distance.md):

$$
d_T(x,B)=\sup_{\substack{\alpha_i\geq0\\\sum_i\alpha_i^2\leq1}}
\inf_{y\in B}\sum_{i:x_i\ne y_i}\alpha_i,\qquad
d_T(A,B)=\inf_{x\in A}d_T(x,B).
$$

Here a coordinate is an entire sampled point, so $x_i\ne y_i$ means the two planar points differ. This is the distance from the upper event $A$ to the lower event $B$; its order is relevant because the convex distance need not be symmetric.

Fix $x\in A$ and choose exactly $a$ indices $I$ whose points form a [convex chain](../../../../../../convex-chain.md) with the endpoints. Such a choice exists even if $L_n(x)>a$, by taking a subchain. It is a certificate of the [certifiable function](../../../../../../certifiable-function.md) $L_n$. For any $y\in B$, let $J=\{i\in I:x_i\ne y_i\}$. The $a-|J|$ unchanged selected points remain a [convex chain](../../../../../../convex-chain.md) in configuration $y$, so

$$
a-|J|\leq L_n(y)\leq b,\qquad |J|\geq a-b.
$$

Choose the nonnegative weights $\alpha_i=a^{-1/2}$ for $i\in I$ and zero otherwise. They have squared sum one, and for every $y\in B$,

$$
\sum_{i:x_i\ne y_i}\alpha_i=\frac{|J|}{\sqrt a}\geq\frac{a-b}{\sqrt a}.
$$

Taking the infimum over $y$, then the supremum over weights, and finally the infimum over $x\in A$ proves

$$
\boxed{d_T(A,B)\geq\frac{a-b}{\sqrt a}.}
$$

This proof also works for $b=0$ if zero-length chains are admitted, and gives the usual infinite separation when one of the events is empty. For the uniform sampling model, $L_n\geq1$ [almost surely](../../../../../../almost-sure-convergence.md) when $n\geq1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

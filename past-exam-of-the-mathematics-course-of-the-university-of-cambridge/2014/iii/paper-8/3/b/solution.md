<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The answer is the [monotone rearrangement](../../../../../../monotone-rearrangement.md)

$$
\boxed{T(x)=G^{-1}(F(x)),\qquad \pi=(\operatorname{Id},T)_*\mu.}
$$

It pushes $\mu$ to $\nu$ by the same cumulative-distribution argument as in part (a).

For the squared [transport cost](../../../../../../transport-cost-function.md), the two-point swap difference is

$$
(y_1-x_1)^2+(y_2-x_2)^2-(y_2-x_1)^2-(y_1-x_2)^2
=-2(x_2-x_1)(y_2-y_1).
$$

Thus any optimal support has no crossed pairs: $x_1<x_2$ forces $y_1\le y_2$. This follows from the finite-cost converse proved above; every cost here is bounded. Conversely, an increasing graph is [c-cyclically monotone](../../../../../../c-cyclical-monotonicity.md) for this cost. After removing the marginal terms $\sum x_i^2+\sum y_i^2$, the cycle inequalities say that pairing the sorted $x_i$ and $y_i$ maximizes $\sum x_iy_i$. Exchanging any inverted pairing increases that sum by the nonnegative product of the two differences, so repeated exchanges prove the inequality. Therefore the displayed increasing transport is optimal.

For uniqueness, let $\pi$ be any noncrossing coupling. The sets $A=\{x\le a\}$ and $B=\{y\le b\}$ cannot both have positive mass in $A\setminus B$ and $B\setminus A$: a point from each would give a strictly crossed pair. Consequently one of these differences has zero mass, and

$$
\pi\{x\le a,y\le b\}=\min\{F(a),G(b)\}.
$$

This determines the joint distribution uniquely and is exactly the distribution of the common-quantile coupling $(F^{-1}(U),G^{-1}(U))$ for uniform $U$. Since $F$ is continuous and strictly increasing, that coupling is induced by $T=G^{-1}F$. Hence **there is one optimal deterministic plan, with maps differing only on $\mu$-null sets**; in fact it is the unique optimal coupling. This proves the [one-dimensional quadratic transport uniqueness criterion](../../../../../../one-dimensional-quadratic-transport-uniqueness-criterion.md) directly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

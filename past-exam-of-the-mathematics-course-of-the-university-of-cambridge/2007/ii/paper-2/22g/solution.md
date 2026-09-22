<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

Let $B_X$ be the open unit ball. Since $T(X)=\bigcup_{n\ge1}T(nB_X)$ is not meagre in $Y$, at least one closure $\overline{T(nB_X)}$ has nonempty interior. A ball contained in that closure, subtracted from itself, gives a ball about zero contained in $\overline{T(2nB_X)}$. Scaling yields some $\delta>0$ with

$$
B_Y(0,\delta)\subseteq\overline{T(B_X)}.
$$

No completeness of $Y$ is used here; the hypothesis is second category in $Y$, not merely in the relative image topology.

If $\|y\|<\delta/2$, choose $x_1\in\tfrac12B_X$ with $\|y-Tx_1\|<\delta/4$. Then choose $x_2\in\tfrac14B_X$ so the new residual is below $\delta/8$, and continue. The series $\sum_jx_j$ converges in the [Banach space](../../../../../banach-space-split.md) $X$, has norm less than one, and continuity of $T$ gives $T(\sum_jx_j)=y$. Thus $B_Y(0,\delta/2)\subseteq T(B_X)$.

The linear subspace $T(X)$ contains a ball about zero, so it is all of $Y$: **$T$ is surjective**. Translated and scaled unit-ball images show that every open-set image is open. If $T$ is injective, its inverse is linear and the ball inclusion gives $\|T^{-1}y\|\le(2/\delta)\|y\|$, by scaling and taking a limiting bound. Thus **$T^{-1}$ exists and is bounded**.

For the first nonlinear counterexample use $f(x)=e^x$: its image $(0,\infty)$ is of second category but is not all of $\mathbb R$. For the second use the continuous surjection $f(x)=x+1$ for $x\le-1$, $f(x)=0$ for $-1\le x\le1$, and $f(x)=x-1$ for $x\ge1$. The open interval $(-1/2,1/2)$ maps to the nonopen singleton $\{0\}$. Linearity is essential to the conclusions.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

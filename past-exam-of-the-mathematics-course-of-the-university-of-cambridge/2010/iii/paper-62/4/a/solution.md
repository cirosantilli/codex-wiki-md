<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $s_j=t_{i+j}$ for $0\le j\le k$, with the knots in increasing order. The explicit formula for a [divided difference](../../../../../../divided-difference.md) at distinct nodes gives

$$
M_i(t)=k\sum_{j=0}^k\frac{(s_j-t)_+^{k-1}}{\prod_{\ell\ne j}(s_j-s_\ell)}.
$$

Each [truncated power function](../../../../../../truncated-power-function.md) is a [piecewise polynomial function](../../../../../../piecewise-polynomial-function.md) of degree $k-1$ and is $C^{k-2}$ for $k\ge2$. Therefore their sum has the same global smoothness. The jump in the $(k-1)$st [derivative](../../../../../../derivative.md) at $s_j$ equals

$$
\frac{k(-1)^k(k-1)!}{\prod_{\ell\ne j}(s_j-s_\ell)},
$$

which is nonzero. Thus each $s_j$ really is a knot, and generally there is no additional smoothness.

If $t<s_0$, the values being differenced are the values of the degree-$k-1$ [polynomial](../../../../../../polynomial-split.md) $(s-t)^{k-1}$, so their $k$th [divided difference](../../../../../../divided-difference.md) vanishes. If $t>s_k$, every sampled [truncated power function](../../../../../../truncated-power-function.md) is zero. To check that both support endpoints occur, for $s_0<t<s_1$ subtract the vanished full [polynomial](../../../../../../polynomial-split.md) divided difference to obtain

$$
M_i(t)=\frac{k(t-s_0)^{k-1}}{\prod_{\ell=1}^k(s_\ell-s_0)}>0.
$$

For $s_{k-1}<t<s_k$, only the last term survives and is positive. The nonnegativity from the recurrence in (b) actually gives positivity throughout the interior: for each $s_0<t<s_k$, at least one lower-order [B-spline](../../../../../../b-spline.md) covering $t$ has a positive recurrence coefficient, and induction starts with positive order-one indicators. Hence **$\operatorname{supp}M_i=[t_i,t_{i+k}]$ and $M_i\in C^{k-2}$ for $k\ge2$**, with degree $k-1$ on its knot intervals. For $k=1$, the [B-spline](../../../../../../b-spline.md) is the step function $1_{[s_0,s_1)}(t)/(s_1-s_0)$, so no continuity is asserted.

The [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md) also follows directly: integrating $k(s_j-t)_+^{k-1}$ over $s_0\le t\le s_k$ gives $(s_j-s_0)^k$. The $k$th [divided difference](../../../../../../divided-difference.md) of this monic degree-$k$ [polynomial](../../../../../../polynomial-split.md) is one. Thus $\int M_i(t)\,dt=1$, explaining its normalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

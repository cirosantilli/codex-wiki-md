<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a continuous vector [semimartingale](../../../../../../semimartingale.md) $X$ and $f\in C^{1,2}$, the **[Itô formula](../../../../../../ito-s-lemma.md)** is

$$
\boxed{f(t,X_t)=f(0,X_0)+\int_0^t\partial_s f(s,X_s)ds+\sum_i\int_0^t\partial_i f(s,X_s)dX_s^i+\frac12\sum_{i,j}\int_0^t\partial_{ij}f(s,X_s)d[X^i,X^j]_s.}
$$

The **[Itô product rule](../../../../../../ito-product-rule.md)**, or stochastic [integration by parts](../../../../../../integration-by-parts.md), is

$$
\boxed{X_tY_t=X_0Y_0+\int_0^tX_s\,dY_s+\int_0^tY_s\,dX_s+[X,Y]_t.}
$$

The additional second-order term is the [quadratic covariation](../../../../../../quadratic-covariation.md).

For general [semimartingales](../../../../../../semimartingale.md) with [càdlàg](../../../../../../cadlag.md) paths, use left limits in the integrands. The **[Itô formula for semimartingales with jumps](../../../../../../ito-formula-for-semimartingales-with-jumps.md)**, for time-independent $f\in C^2$, is

$$
f(X_t)=f(X_0)+\sum_i\int_0^t\partial_i f(X_{s-})dX_s^i+\frac12\sum_{i,j}\int_0^t\partial_{ij}f(X_{s-})d[X^{i,c},X^{j,c}]_s+\sum_{0<s\leq t}\left(f(X_s)-f(X_{s-})-\sum_i\partial_i f(X_{s-})\Delta X_s^i\right).
$$

Here $X^c$ denotes the continuous [local martingale](../../../../../../local-martingale.md) part; the continuous bracket is that of these parts. For time-dependent $f\in C^{1,2}$ add $\int\partial_s f(s,X_{s-})ds$ and insert $s$ in the other evaluations of $f$. The [integration by parts](../../../../../../integration-by-parts.md) formula becomes

$$
X_tY_t=X_0Y_0+\int_0^tX_{s-}dY_s+\int_0^tY_{s-}dX_s+[X,Y]_t,\qquad [X,Y]_t=[X^c,Y^c]_t+\sum_{0<s\leq t}\Delta X_s\Delta Y_s.
$$

For continuous paths the jump sum vanishes, recovering the first two formulas.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

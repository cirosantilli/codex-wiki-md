<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [càdlàg](../../../../../../cadlag.md) [semimartingales](../../../../../../semimartingale.md), the [semimartingale integration by parts](../../../../../../semimartingale-integration-by-parts.md) formula is

$$
\boxed{X_tY_t=X_0Y_0+\int_0^tX_{s-}\,dY_s+\int_0^tY_{s-}\,dX_s+[X,Y]_t.}
$$

For continuous processes the left limits can be replaced by the values. The bracket includes the jump products in the general formula.

For a continuous $\mathbb R^d$-valued [semimartingale](../../../../../../semimartingale.md) $X$ and $f\in C^2(\mathbb R^d)$, the [Itô formula](../../../../../../ito-s-lemma.md) is

$$
\boxed{f(X_t)=f(X_0)+\sum_{i=1}^d\int_0^t\partial_if(X_s)\,dX_s^i+\frac12\sum_{i,j=1}^d\int_0^t\partial_{ij}f(X_s)\,d[X^i,X^j]_s.}
$$

The formula is localized when the derivatives are unbounded; continuity of $X$ makes them bounded after stopping on compact sets.

To prove the one-dimensional formula for polynomials without assuming that formula, use induction. It is immediate for constants and $X$. Suppose

$$
d(X^k)=kX^{k-1}\,dX+\frac{k(k-1)}2X^{k-2}\,d[X].
$$

Write $X=X_0+M+A$ with $M$ a [continuous local martingale](../../../../../../continuous-local-martingale.md) and $A$ [finite variation](../../../../../../total-variation-of-a-function.md). The induction hypothesis identifies the [martingale](../../../../../../martingale-split.md) part of $X^k$ as $kX^{k-1}\cdot M$. The stochastic-integral covariation identity, obtained by polarization from the quadratic-variation identity, gives

$$
d[X^k,X]=kX^{k-1}\,d[X].
$$

Apply [semimartingale integration by parts](../../../../../../semimartingale-integration-by-parts.md) to $X^kX$. Its first-order terms combine to $(k+1)X^k\,dX$, and its bracket terms combine to

$$
\left(\frac{k(k-1)}2+k\right)X^{k-1}\,d[X]=\frac{k(k+1)}2X^{k-1}\,d[X].
$$

This proves the induction step. Taking linear combinations proves the [polynomial Itô formula from integration by parts](../../../../../../polynomial-ito-formula-from-integration-by-parts.md) for every polynomial $f$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

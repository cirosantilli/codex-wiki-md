<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The relevant [invariance principle for a low-degree multilinear polynomial](../../../../../../invariance-principle-for-a-low-degree-multilinear-polynomial.md) is the following. Let $(X_i)$ and $(Y_i)$ be sequences of [independent random variables](../../../../../../independent-random-variables.md) satisfying

$$
\mathbb E X_i=\mathbb E Y_i=0,
\quad
\mathbb E X_i^2=\mathbb E Y_i^2=1,
\quad
\mathbb E X_i^3=\mathbb E Y_i^3=0,
\quad
\mathbb E X_i^4,\mathbb E Y_i^4\leq9.
$$

If $f$ is multilinear of degree at most $k$ and $\lVert\psi^{(4)}\rVert_\infty\leq M$, then

$$
|\mathbb E\psi(f(X))-\mathbb E\psi(f(Y))|
\leq\frac M{12}9^k\sum_{i=1}^n\operatorname{Inf}_i(f)^2.
$$

For the proof, use the [Lindeberg replacement method](../../../../../../lindeberg-replacement-method.md). Replace $X_i$ by $Y_i$ one coordinate at a time and write $f=u_i+z_iv_i$, where $u_i=E_i f$ and $v_i=D_i f$ depend only on the other coordinates. A third-order [Taylor expansion](../../../../../../taylor-theorem.md) of $\psi(u_i+z_iv_i)$ has identical expected terms through order three for $z_i=X_i$ and $z_i=Y_i$, because the first three moments match. Each fourth-order remainder is bounded by $M|z_iv_i|^4/24$, so the $i$th replacement costs at most

$$
\frac M{24}(\mathbb E X_i^4+\mathbb E Y_i^4)\mathbb E v_i^4.
$$

Part (i), applied in the hybrid product space, bounds each of the two fourth-moment terms by $9^k\operatorname{Inf}_i(f)^2$. Thus the cost is at most $(M/12)9^k\operatorname{Inf}_i(f)^2$. The [triangle inequality](../../../../../../triangle-inequality.md) and summation over $i$ prove the result.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

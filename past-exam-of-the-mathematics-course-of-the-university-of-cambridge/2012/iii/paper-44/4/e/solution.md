<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $D=\mathbb E\int_0^\infty e^{-bt/R}Z_t^{1-1/R}\,dt$ and use the [product measure](../../../../../../product-measure.md) $d\mathbb P\,dt$. For $0<R<1$, the [conjugate exponents](../../../../../../conjugate-exponents.md) are $p=1/(1-R)$ and $q=1/R$. Factor the utility integrand as

$$
e^{-bt}c_t^{1-R}=(Z_tc_t)^{1-R}\bigl(e^{-bt}Z_t^{R-1}\bigr).
$$

The [Holder inequality](../../../../../../holder-inequality.md) on this [product measure](../../../../../../product-measure.md) gives

$$
\mathbb E\int_0^\infty e^{-bt}c_t^{1-R}\,dt\leq\left(\mathbb E\int_0^\infty Z_tc_t\,dt\right)^{1-R}D^R\leq X_0^{1-R}D^R.
$$

Divide by $1-R$ to obtain the [Hölder bound for discounted CRRA consumption](../../../../../../holder-bound-for-discounted-crra-consumption.md):

$$
\boxed{\mathbb E\int_0^\infty e^{-bt}U(c_t)\,dt\leq U(X_0)\left[\mathbb E\int_0^\infty e^{-bt/R}Z_t^{1-1/R}\,dt\right]^R.}
$$

For a finite right side this is ordinary Hölder; on the infinite measure space one can first truncate time and then pass by [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). If $D=\infty$ and $X_0>0$, the bound is valid but uninformative. If $X_0=0$, the budget forces $c=0$ almost everywhere, so the utility integral is zero; handle this separately instead of writing an undefined $0\cdot\infty$.

When $D$ is finite and the bound is attained, equality requires full budget use and $c_t=(X_0/D)e^{-bt/R}Z_t^{-1/R}$. This is the equality pattern of Hölder, not an assertion that every market can finance that process.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

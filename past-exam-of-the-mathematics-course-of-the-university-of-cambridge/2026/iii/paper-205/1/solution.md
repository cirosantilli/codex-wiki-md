<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With the usual objective

$$
\frac1{2n}\lVert Y-\widehat\mu\mathbf1-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_1,
$$

the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) for the [Lasso](../../../../../lasso.md) are

$$
\frac1nX^T(Y-\widehat\mu\mathbf1-X\widehat\beta_\lambda)=\lambda z,
\quad
z_j=\operatorname{sgn}(\widehat\beta_{\lambda j})\text{ if }\widehat\beta_{\lambda j}\ne0,
\quad |z_j|\leq1\text{ otherwise}.
$$

Comparing the objective at $\widehat\beta_\lambda$ and $\beta^0$, expanding the square, and cancelling the noise norm gives exactly

$$
\frac1n\lVert X(\beta^0-\widehat\beta_\lambda)\rVert_2^2
\leq\frac1n\varepsilon^TX(\widehat\beta_\lambda-\beta^0)
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta_\lambda\rVert_1.
$$

Choose $\lambda=A\sigma\sqrt{\log p/n}$. Since every column has norm $\sqrt n$, each $X_j^T\varepsilon/n$ is [sub-Gaussian](../../../../../sub-gaussian-distribution.md) with parameter $\sigma/\sqrt n$. A [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P\!\left(\left\lVert\frac1nX^T\varepsilon\right\rVert_\infty>\lambda\right)
\leq2p\exp\!\left(-\frac{n\lambda^2}{2\sigma^2}\right)
=2p^{-(A^2/2-1)}.
$$

On the complementary event, [Holder inequality](../../../../../holder-inequality.md) and the triangle inequality bound the preceding right-hand side by

$$
\lambda\lVert\widehat\beta_\lambda-\beta^0\rVert_1
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta_\lambda\rVert_1
\leq2\lambda\lVert\beta^0\rVert_1,
$$

which proves the stated prediction bound.

For the [Dantzig selector](../../../../../dantzig-selector.md), use the constraint $n^{-1}\lVert X^T(Y-X\beta)\rVert_\infty\leq\lambda$. The Lasso KKT conditions make $\widehat\beta_\lambda$ feasible, so a Dantzig minimizer $\widetilde\beta$ has no larger $\ell^1$ norm. If $\widetilde\beta$ were not the Lasso solution, uniqueness from invertibility of $X^TX$ would imply that some active coordinate $j$ has strict signed KKT slack. For small $\eta>0$, set

$$
\beta_\eta=\widetilde\beta-eta\operatorname{sgn}(\widetilde\beta_j)(X^TX)^{-1}e_j.
$$

Only score coordinate $j$ changes, toward its feasible boundary, so $\beta_\eta$ remains feasible. For small $\eta$, signs on the active coordinates do not change, and

$$
\lVert\beta_\eta\rVert_1-\lVert\widetilde\beta\rVert_1
\leq\eta\left(-[(X^TX)^{-1}]_{jj}+\sum_{k\ne j}|[(X^TX)^{-1}]_{kj}|\right)<0
$$

by strict [diagonal dominance](../../../../../diagonal-dominance.md). This contradicts Dantzig optimality, so the two estimators coincide.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

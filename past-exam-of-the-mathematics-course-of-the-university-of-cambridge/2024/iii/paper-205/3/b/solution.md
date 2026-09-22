<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\delta=\widehat\beta-\beta^0$. On $\Omega$, [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\frac1n\delta^TX^T\varepsilon
\leq\lVert\delta\rVert_1\frac{\lVert X^T\varepsilon\rVert_\infty}{n}
\leq\frac\lambda2\lVert\delta\rVert_1.
$$

Since $\beta_N^0=0$, the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1
\leq\lVert\delta_S\rVert_1-\lVert\delta_N\rVert_1.
$$

Substitution in the [Basic inequality for the Lasso](../../../../../../basic-inequality-for-the-lasso.md), followed by discarding the nonnegative prediction-error term, yields

$$
\frac\lambda2\lVert\delta_N\rVert_1
\leq\frac{3\lambda}{2}\lVert\delta_S\rVert_1.
$$

**Therefore $\lVert\widehat\beta_N-\beta_N^0\rVert_1\leq3\lVert\widehat\beta_S-\beta_S^0\rVert_1$, the [Lasso cone condition](../../../../../../lasso-cone-condition.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

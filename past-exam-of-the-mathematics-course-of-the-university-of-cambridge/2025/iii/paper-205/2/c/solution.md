<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $s=\lVert\widehat\beta\rVert_0+\lVert\beta^0\rVert_0$. Since $\delta$ has at most $s$ nonzero coordinates, $\lVert\delta\rVert_1^2\leq s\lVert\delta\rVert_2^2$. On $\Omega_2$,

$$
\delta^T\widehat\Sigma\delta
\geq\delta^T\Sigma^0\delta-
\lVert\widehat\Sigma-\Sigma^0\rVert_\infty\lVert\delta\rVert_1^2
\geq\frac\mu2\lVert\delta\rVert_2^2,
$$

where $\widehat\Sigma=X^TX/n$. Write $R=\delta^T\widehat\Sigma\delta$. On $\Omega_1$,

$$
R\leq2A\sigma v\sqrt{\frac{\log p}{n}}\lVert\delta\rVert_1
\leq2A\sigma v\sqrt{\frac{2s\log p}{\mu n}}\sqrt R.
$$

Squaring after division by $\sqrt R$ proves

$$
\boxed{\frac1n\lVert X(\beta^0-\widehat\beta)\rVert_2^2
\leq8A^2\sigma^2v^2\frac{s\log p}{\mu n}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

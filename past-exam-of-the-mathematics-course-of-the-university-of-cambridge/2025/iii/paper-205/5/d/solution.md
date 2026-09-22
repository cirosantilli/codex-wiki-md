<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $x_*\sim N_p(0,I)$ is independent, conditional prediction risk equals $\mathbb E(\lVert\widehat\beta_\lambda-\beta^0\rVert_2^2\mid X)$. With $\widehat\Sigma=X^TX/n$ and $\lambda=n\ell$,

$$
\widehat\beta_\lambda-\beta^0
=-\ell(\widehat\Sigma+\ell I)^{-1}\beta^0
+\frac1n(\widehat\Sigma+\ell I)^{-1}X^T\varepsilon.
$$

The noise term has conditional mean zero and covariance $\frac{\sigma^2}{n}\,(\widehat\Sigma+\ell I)^{-1}\widehat\Sigma(\widehat\Sigma+\ell I)^{-1}$. Taking squared norms proves

$$
\boxed{R_X(\widehat\beta_\lambda)=
\ell^2(\beta^0)^T(\widehat\Sigma+\ell I)^{-2}\beta^0
+\frac{\sigma^2}{n}\operatorname{tr}\bigl(\widehat\Sigma(\widehat\Sigma+\ell I)^{-2}\bigr).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

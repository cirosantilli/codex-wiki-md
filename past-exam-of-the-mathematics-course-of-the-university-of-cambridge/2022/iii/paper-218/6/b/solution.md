<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With unit error variance, the [Gaussian likelihood](../../../../../../gaussian-likelihood.md) has log-likelihood

$$
\ell(\beta)
=-\frac n2\log(2\pi)-\frac12\|Y-X\beta\|_2^2.
$$

Full column rank gives $\widehat\beta=(X^TX)^{-1}X^TY$ and the least-squares identity

$$
\|Y-X\beta\|_2^2
=\|Y-X\widehat\beta\|_2^2
+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta).
$$

Multiplying the likelihood by $\prod_j\phi(\beta_j)$ and absorbing all terms independent of $\beta$ into $C$ gives

$$
\boxed{\pi(\beta\mid Y)
=C\exp\left[
-\frac12(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)
+\sum_{j=1}^p\log\phi(\beta_j)
\right].}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

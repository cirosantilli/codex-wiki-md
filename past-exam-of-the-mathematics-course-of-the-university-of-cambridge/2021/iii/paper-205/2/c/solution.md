<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $\lVert X_j\rVert_2=\sqrt n$, each coordinate of $X^T\varepsilon/n$ is $N(0,\sigma^2/n)$. The [Gaussian tail bound](../../../../../../gaussian-tail-bound.md) and a [union bound](../../../../../../boole-s-inequality.md) give

$$
\mathbb P\left(\left\lVert\frac{X^T\varepsilon}{n}\right\rVert_\infty>\frac\lambda2\right)
\leq2p\exp\left(-\frac{n\lambda^2}{8\sigma^2}\right)
=2p^{-(A^2/8-1)}.
$$

On the complementary score event, the standard [Basic inequality for the Lasso](../../../../../../basic-inequality-for-the-lasso.md), cone argument, and compatibility oracle inequality give, for $S=\operatorname{supp}(\beta^0)$,

$$
\frac1n\lVert X(\widehat\beta-\beta^0)\rVert_2^2
+\lambda\lVert\widehat\beta-\beta^0\rVert_1
\leq\frac{16\lambda^2s}{\phi_{\widehat\Sigma}^2(S)}.
$$

Using part b and $\lambda^2=A^2\sigma^2\log p/n$ proves

$$
\boxed{
\frac1n\lVert X(\widehat\beta-\beta^0)\rVert_2^2
+\lambda\lVert\widehat\beta-\beta^0\rVert_1
\leq\frac{32A^2\sigma^2\log p}{\eta}\frac{s}{n}}
$$

with the required probability.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

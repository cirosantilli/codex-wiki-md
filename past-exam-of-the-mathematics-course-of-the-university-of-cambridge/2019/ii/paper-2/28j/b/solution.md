<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The mass function is the mixture

$$
p_{\pi,\lambda}=(1-\pi)\delta_0
+\pi\operatorname{Poisson}(\lambda),
$$

so it is nonnegative and sums to one. Its first two moments are

$$
\mathbb E[Y]=\pi\lambda,
\qquad
\mathbb E[Y^2]=\pi(\lambda+\lambda^2).
$$

Therefore

$$
\operatorname{Var}(Y)
=\pi\lambda+\pi(1-\pi)\lambda^2.
$$

For $0<\pi<1$ this is strictly larger than the mean, so the [Zero-inflated Poisson distribution](../../../../../../zero-inflated-poisson-distribution.md) models overdispersion. At $\pi=1$ it reduces to an ordinary Poisson distribution, and at $\pi=0$ it is degenerate at zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

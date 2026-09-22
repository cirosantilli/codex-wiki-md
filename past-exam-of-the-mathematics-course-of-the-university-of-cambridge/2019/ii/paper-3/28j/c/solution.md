<h1 id="28j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $S_n/n=\overline X\to1/\theta$ almost surely, and hence in probability. Therefore

$$
\widehat\theta_\pi
=\frac{1+\alpha/n}{\overline X+\beta/n}
\xrightarrow{p}\theta
$$

by the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md). Thus the Bayes estimator has [statistics](../../../../../../consistency-statistics.md).

It differs from the maximum-likelihood estimator by

$$
\widehat\theta_\pi-\widehat\theta_{\rm MLE}
=\frac{\alpha S_n-n\beta}{S_n(S_n+\beta)}.
$$

Since $S_n/n\to1/\theta$, the numerator is $O_p(n)$ and the denominator is $O_p(n^2)$, so this difference is $O_p(n^{-1})=o_p(n^{-1/2})$. The limit in part a and [Slutsky theorem](../../../../../../slutsky-theorem.md) now give

$$
\boxed{
\sqrt n(\widehat\theta_\pi-\theta)
\xrightarrow dN(0,\theta^2).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

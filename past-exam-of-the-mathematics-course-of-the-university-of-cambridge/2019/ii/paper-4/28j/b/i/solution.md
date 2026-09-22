<h1 id="28j/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md) gives

$$
\boxed{\widehat\mu_n=\frac1n\sum_{i=1}^nh(X_i)
\longrightarrow\mathbb E_{\theta_0}[h(X)]=\mu(\theta_0)
\quad\text{almost surely}.}
$$

A continuous one-to-one real function is strictly monotone and has a continuous inverse on its image. Hence

$$
\boxed{\widehat\theta_n=\mu^{-1}(\widehat\mu_n)}
$$

whenever $\widehat\mu_n$ lies in that image; an arbitrary extension outside the image handles the remaining finite-sample values. The [continuous mapping theorem](../../../../../../../continuous-mapping-theorem.md) gives $\widehat\theta_n\to\theta_0$ almost surely, so this is a [consistent estimator](../../../../../../../consistency-statistics.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [28J](../../../28j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Watterson estimator](../../../../../../watterson-estimator.md) is

$$
\boxed{\widehat\theta=\frac{S}{H_{n-1}}.}
$$

The expectation above makes it an [unbiased estimator](../../../../../../unbiased-estimator.md). Its [variance](../../../../../../variance-split.md), given by the [variance of the Watterson estimator](../../../../../../variance-of-the-watterson-estimator.md), is

$$
\mathbb E(\widehat\theta-\theta)^2=\frac{\theta}{H_{n-1}}+\frac{\theta^2H_{n-1}^{(2)}}{H_{n-1}^2}\longrightarrow0.
$$

Indeed, the [harmonic sum](../../../../../../harmonic-sum.md) satisfies $H_{n-1}\sim\log n$ and $H_{n-1}^{(2)}$ stays bounded. This proves [mean-square convergence](../../../../../../convergence-in-l2.md); the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) then shows that it is a [consistent estimator](../../../../../../consistency-statistics.md), since $P(|\widehat\theta-\theta|>\varepsilon)\le\operatorname{Var}(\widehat\theta)/\varepsilon^2\to0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

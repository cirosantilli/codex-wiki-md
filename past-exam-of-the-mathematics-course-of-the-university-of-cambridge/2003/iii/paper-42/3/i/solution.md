<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take logarithms entry by entry before centering. For tree $i$, let $z_i=(\log G_i,\log H_i,\log V_i)^T$, and put $\bar z=31^{-1}\sum_i z_i$. The command `var(log(b))` computes the [sample covariance matrix](../../../../../../sample-covariance-matrix.md) with the [unbiased estimator](../../../../../../unbiased-estimator.md) normalization

$$
\boxed{\widehat\Sigma=\frac1{30}\sum_{i=1}^{31}(z_i-\bar z)(z_i-\bar z)^T.}
$$

Thus entry $(j,k)$ is the sum of products of the centered log measurements divided by $30$, not the logarithm of the covariance between the original measurements. Its diagonal entries are the three log-variable [sample variances](../../../../../../sample-variance.md), and the off-diagonal entries are their [sample covariances](../../../../../../sample-covariance.md). The positive off-diagonal entries indicate positive association of the log measurements. Taking logarithms turns a multiplicative relation such as $V\approx cG^2H$ into the approximately linear relation $\log V\approx\log c+2\log G+\log H$, which motivates investigating [principal components](../../../../../../principal-component.md) of these transformed observations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat the simulated pairs $(x_i,m_i)$ as samples from the prior $P(x,m)$. The numerator and denominator of the posterior mean are then ordinary [Monte Carlo estimators](../../../../../../monte-carlo-estimator.md), so

$$
\bar m\simeq\frac{\sum_{i=1}^Km_iP(d\mid x_i)}
{\sum_{j=1}^KP(d\mid x_j)}
=\sum_{i=1}^Km_iw_i,
$$

where the normalized [importance sampling](../../../../../../importance-sampling.md) weights are

$$
\boxed{w_i=\frac{\exp[-(d-x_i)^2/(2\sigma^2)]}
{\sum_{j=1}^K\exp[-(d-x_j)^2/(2\sigma^2)]}.}
$$

The common Gaussian normalizing constant cancels.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

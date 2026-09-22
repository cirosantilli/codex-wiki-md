<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The variance $\mu+\mu^2/\theta$ approaches the [Poisson distribution](../../../../../../poisson-distribution.md) variance $\mu$ when $\theta\to\infty$. Equivalently, with $\alpha=1/\theta\geq0$, the Poisson model is the boundary value $\alpha=0$. The usual [Wilks theorem](../../../../../../wilks-theorem.md) for a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) assumes that the null parameter is an interior point of a smooth parameter space, so comparing the statistic with an ordinary $\chi_1^2$ law is invalid here.

A valid [parametric bootstrap](../../../../../../parametric-bootstrap.md) proceeds as follows. First fit the null Poisson model and retain its fitted means $\widehat\mu_i$. For each bootstrap repetition $b=1,\ldots,B$, independently simulate

$$
Y_i^{(b)}\sim\operatorname{Pois}(\widehat\mu_i),
$$

using the original doses, refit both the Poisson and negative-binomial models to that simulated data, and calculate

$$
T_b=2\left\{\ell_{NB}^{(b)}-\ell_P^{(b)}\right\}.
$$

For the observations calculate the analogous $T_{obs}$. The bootstrap $p$-value

$$
\widehat p=\frac{1+\sum_{b=1}^B\mathbf1_{\{T_b\geq T_{obs}\}}}{B+1}
$$

uses the null distribution with its boundary and finite-sample fitting behaviour automatically reproduced. A large $B$ controls the [Monte Carlo error](../../../../../../monte-carlo-error.md) of this estimate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

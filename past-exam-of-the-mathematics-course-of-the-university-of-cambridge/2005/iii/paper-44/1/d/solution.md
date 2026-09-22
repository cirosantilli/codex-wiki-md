<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Differentiating the [log-likelihood](../../../../../../log-likelihood.md) again gives

$$
\boxed{\ell''(\theta)=-\frac{D}{\theta^2},\qquad
J(\theta):=-\ell''(\theta)=\frac{D}{\theta^2}.}
$$

Thus the [Observed Fisher information](../../../../../../observed-fisher-information.md) for the rate is proportional to the total number of observed events. At a positive interior [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), the large-sample variance estimate and [standard error](../../../../../../standard-error.md) are

$$
\widehat{\operatorname{Var}}(\widehat\theta)=J(\widehat\theta)^{-1}
=\frac{\widehat\theta^2}{D},\qquad
\operatorname{se}(\widehat\theta)\simeq\frac{\widehat\theta}{\sqrt D}.
$$

Precision is therefore driven by the number of observed events rather than by the number recruited alone. Heavy [right censoring](../../../../../../right-censoring.md) can leave a large study with little information about its [hazard function](../../../../../../hazard-function.md). Under the regularity conditions for the [Fisher information](../../../../../../fisher-information-matrix.md), the expected information is $\mathbb E[D]/\theta^2$.

A [right-censored](../../../../../../right-censoring.md) observation is not wholly uninformative: its exposure contributes to $E$, changes the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), and affects the expected number of events under a sampling design. Its contribution $-\theta x_i$ happens to have zero second derivative in this rate parameterization. For example, if no events occur, the likelihood still declines as $e^{-\theta E}$ and disfavors large rates, despite its zero curvature. The usual interior variance approximation is then invalid.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

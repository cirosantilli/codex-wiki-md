<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The moment-based approach specifies marginal means, [variances](../../../../../../variance-split.md), and within-student [covariances](../../../../../../covariance.md), without supplying a joint probability distribution for each count profile. It is a [quasi-likelihood](../../../../../../quasi-likelihood.md) or [generalized estimating equation](../../../../../../generalized-estimating-equation.md) strategy. The parameter interpreted as a structural-zero fraction is not automatically an actual probability of a [structural-zero component](../../../../../../count-mixture-structural-zero.md) merely because it appears in the moment formulas. A valid positive-definite working [covariance](../../../../../../covariance.md) and parameter [identifiability](../../../../../../identifiability.md) must also be checked.

The printed covariance specification is not admissible for all the stated parameter values. For example, take $\pi=1/2$, $\tau=1$, and all three component means equal to 10. It gives diagonal [variance](../../../../../../variance-split.md) 80 and off-diagonal [covariance](../../../../../../covariance.md) 100, so $\operatorname{Var}(Y_{i1}-Y_{i2})=80+80-2(100)=-40$. A [covariance matrix](../../../../../../covariance-matrix.md) cannot have a negative variance in any direction. Thus the moment approach requires additional admissibility restrictions or a valid working covariance; the parameter ranges alone do not define a valid model. This does not alter the hierarchical model, whose covariance derived below is positive semidefinite.

The alternative gives a full hierarchical [mixture distribution](../../../../../../mixture-distribution.md), specifically a [shared zero-inflated Gamma-Poisson count model](../../../../../../shared-zero-inflated-gamma-poisson-count-model.md): a common student [random effect](../../../../../../random-effect.md) is zero with probability $\pi$, and otherwise has a [Gamma distribution](../../../../../../gamma-distribution.md) with mean 1 and [variance](../../../../../../variance-split.md) $\tau$. Conditional on this effect, the three counts are independent [Poisson random variables](../../../../../../poisson-distribution.md). Integrating it out induces both excess zeros and positive within-student dependence. [Zero inflation](../../../../../../zero-inflation.md) is shared for the whole student, rather than independently reselected in each term. This full distribution supports likelihood-based inference but is more sensitive to the distributional assumptions.

The marginal mean in the hierarchical model has the same form as the proposed moment mean. Its marginal [covariance](../../../../../../covariance.md) does not, in general, equal the printed working [covariance](../../../../../../covariance.md); the [law of total covariance](../../../../../../law-of-total-covariance.md) calculation below makes the distinction explicit. At $\tau=0$ the Gamma component is interpreted as its point-mass-at-one limit. At $\pi=1$ all counts are zero, and the log-mean parameterization and regression effects are not identifiable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

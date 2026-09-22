<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Negative [covariance](../../../../../../covariance.md) can be exploited through [antithetic variates](../../../../../../antithetic-variates.md), but it must belong to an actual joint sampling scheme. Two separately independent samples do not inherit negative [covariance](../../../../../../covariance.md) merely because one can imagine a coupling of their marginal distributions. Interpret the data as $h=\min(n,m)$ independent matched pairs $(X_i,Y_i)$ with [covariance](../../../../../../covariance.md) $\sigma_{XY}<0$, together with independent unmatched observations if the sample sizes differ. Other known pairing schemes can be handled by substituting their actual [covariance](../../../../../../covariance.md) of the two means.

Let $A=\overline X$, $B=\overline Y$, and put

$$
V_X=\sigma_X^2/n,\qquad V_Y=\sigma_Y^2/m,\qquad C=\operatorname{Cov}(A,B)=h\sigma_{XY}/(nm).
$$

For any fixed $w$, the combination $wA+(1-w)B$ is an [unbiased estimator](../../../../../../unbiased-estimator.md) of the common [mean](../../../../../../expected-value.md). Its [variance](../../../../../../variance-split.md) is $w^2V_X+(1-w)^2V_Y+2w(1-w)C$. Differentiation, or [completing the square](../../../../../../completing-the-square.md), gives the [minimum-variance combination of unbiased sample means](../../../../../../minimum-variance-combination-of-unbiased-sample-means.md):

$$
\boxed{\widetilde\theta=w_*A+(1-w_*)B,\qquad
w_*=\frac{V_Y-C}{V_X+V_Y-2C},\qquad
\operatorname{Var}(\widetilde\theta)=\frac{V_XV_Y-C^2}{V_X+V_Y-2C}.}
$$

With $C<0$, both weights are positive. This is efficiency among fixed linear unbiased combinations, not a universal claim about every possible [estimator](../../../../../../estimator.md) for arbitrary distributions $F,G$.

For an immediately implementable exactly [unbiased estimator](../../../../../../unbiased-estimator.md) without known moments, use fixed $w=n/(n+m)$, the pooled [sample mean](../../../../../../sample-mean.md). Its [variance](../../../../../../variance-split.md) is

$$
\frac{n\sigma_X^2+m\sigma_Y^2+2h\sigma_{XY}}{(n+m)^2},
$$

which shows directly the gain from negative [covariance](../../../../../../covariance.md). For any fixed weight, estimate $V_X,V_Y$ using $s_X^2/n,s_Y^2/m$, and $C$ using $h s_{XY}/(nm)$, with $s_{XY}$ the usual unbiased [sample covariance](../../../../../../sample-covariance.md) of the matched pairs. Substitute them into the variance quadratic. At least two matched pairs are needed to estimate their [covariance](../../../../../../covariance.md) nonparametrically.

If the unknown optimal weights are desired while retaining exact unbiasedness, a [cross-fitted combination of unbiased sample means](../../../../../../cross-fitted-combination-of-unbiased-sample-means.md) gives an algorithm using the supplied data. Split the independent pairs and unmatched observations into two folds, keeping each pair together and retaining observations of both types in each fold. Estimate the moments from fold 2 to choose the weight for the fold-1 [sample means](../../../../../../sample-mean.md), adjusting the variance terms for fold 1's sample sizes; do the converse for fold 2. Clip estimated weights to $(0\leq w\leq1)$, to keep them bounded when training moment estimates are unstable. Average the two held-out combinations with deterministic weights, for example one half each for balanced folds.

Conditional on its training fold, each held-out pair of [sample means](../../../../../../sample-mean.md) has [expectation](../../../../../../expected-value.md) $\theta$, and its weights sum to one. Each held-out combination, and hence their average, is therefore exactly an [unbiased estimator](../../../../../../unbiased-estimator.md). Under consistent moment estimation with increasing balanced folds, the weights approach $w_*$ and recover its first-order [variance](../../../../../../variance-split.md) advantage. In contrast, estimating a weight from the same data to which it is applied need not yield an [unbiased estimator](../../../../../../unbiased-estimator.md).

Estimate the [variance](../../../../../../variance-split.md) of this fitted-weight procedure by a [bootstrap](../../../../../../bootstrapping-statistics.md) that resamples matched pairs as blocks and unmatched observations separately, repeats the entire split/weight/combination procedure, and takes the [sample variance](../../../../../../sample-variance.md) of the resulting estimates. This preserves the negative [covariance](../../../../../../covariance.md) and includes variability of the fitted weights. Resampling the $x$ and $y$ values independently would erase the feature responsible for the improvement. The [bootstrap](../../../../../../bootstrapping-statistics.md) estimate has its usual large-sample qualification; the fixed-weight plug-in variance formula above is the simpler alternative when weights are predetermined.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

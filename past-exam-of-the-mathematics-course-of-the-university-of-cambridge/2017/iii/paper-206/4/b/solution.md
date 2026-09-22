<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X$ have columns $1,t$, and let $Z$ have one column per incubator, with entry $t_i$ in the column for observation $i$'s incubator and zeros elsewhere. Integrating the Gaussian [random effects](../../../../../../random-effect.md) gives

$$
Y\sim N(X\beta,V),\qquad V=\sigma^2I+\tau^2ZZ^T.
$$

Consequently its marginal [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta,\sigma^2,\tau^2)=-\frac12\{n\log(2\pi)+\log\det V+(Y-X\beta)^TV^{-1}(Y-X\beta)\}.
$$

The [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) of $H_0:\tau^2=0$ against $\tau^2>0$ uses

$$
\boxed{T=2\left[\sup_{\beta,\sigma^2>0,\tau^2\ge0}\ell-\sup_{\beta,\sigma^2>0}\ell(\beta,\sigma^2,0)\right].}
$$

For each [covariance](../../../../../../covariance.md), the optimizing coefficients are the [generalized least squares](../../../../../../generalized-least-squares.md) estimator $(X^TV^{-1}X)^{-1}X^TV^{-1}Y$. Both fits should use the same marginal likelihood convention, for example fitting the alternative with `update(fly.model, REML=FALSE)` and the null as a Gaussian linear model. The displayed alternative [REML](../../../../../../restricted-maximum-likelihood.md) criterion alone cannot supply $T$.

The [variance](../../../../../../variance-split.md) component is constrained to be nonnegative, and zero lies on the boundary. Thus the interior-parameter hypothesis of [Wilks theorem](../../../../../../wilks-theorem.md) fails; the usual $\chi_1^2$ approximation is inappropriate. A $\tfrac12\delta_0+\tfrac12\chi_1^2$ limit sometimes applies to a single [variance](../../../../../../variance-split.md) component under additional asymptotic conditions, but four incubators do not give a persuasive large-number-of-groups approximation.

Use a [parametric bootstrap](../../../../../../parametric-bootstrap.md) under the null: estimate $\beta,\sigma^2$ there; simulate independent Gaussian errors with that fitted [variance](../../../../../../variance-split.md) at exactly the observed times and grouping labels; refit both models by maximum likelihood for each simulated sample; and calculate $T^*$. The upper-tail proportion, conventionally $(1+\#\{T^*\ge T\})/(B+1)$, estimates the [p-value](../../../../../../p-value.md). Boundary fits with estimated $\tau^2=0$ must remain in the simulation distribution. A restricted-likelihood ratio and a correspondingly calibrated bootstrap are another option when the fixed-effect design is identical, but one must not mix ordinary and restricted likelihoods in a single statistic.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

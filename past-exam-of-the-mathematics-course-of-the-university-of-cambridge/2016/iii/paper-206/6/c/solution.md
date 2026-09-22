<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md) procedure estimates covariance parameters from error contrasts that remove the unknown [fixed effects](../../../../../../fixed-effect.md). Let $X$ have rank $p$ and choose an $n\times(n-p)$ full-rank matrix $A$ with $A^TX=0$. Then $A^TY\sim N(0,A^TV(\vartheta)A)$ has a likelihood involving the variance parameters $\vartheta$ but not $\beta$. Maximizing that likelihood is [restricted maximum likelihood](../../../../../../restricted-maximum-likelihood.md). An equivalent [restricted likelihood from orthogonal error contrasts](../../../../../../restricted-likelihood-from-orthogonal-error-contrasts.md), up to terms independent of $\vartheta$, is

$$
\ell_R(\vartheta)=-\frac12\left[
\log|V|+\log|X^TV^{-1}X|+Y^TP_VY+(n-p)\log(2\pi)\right],
$$

where

$$
P_V=V^{-1}-V^{-1}X(X^TV^{-1}X)^{-1}X^TV^{-1}.
$$

After estimating $\vartheta$, use [generalized least squares](../../../../../../generalized-least-squares.md) for $\widehat\beta=(X^T\widehat V^{-1}X)^{-1}X^T\widehat V^{-1}Y$ and the conditional modes from part (b). In an independent-error [normal linear model](../../../../../../normal-linear-model.md), this covariance procedure reduces to estimating $\sigma^2$ by $\mathrm{RSS}/(n-p)$ instead of $\mathrm{RSS}/n$.

The two models being compared have different fixed-effect spaces, so their error contrasts, dimensions, and restricted likelihoods differ. Their REML values are not likelihoods of the same transformed data and must not be used directly for this fixed-effect [likelihood-ratio test](../../../../../../likelihood-ratio-test.md). **Refit both with ordinary maximum likelihood**, integrating out the [random effects](../../../../../../random-effect.md) but retaining the original response vector, and maximize each model's marginal likelihood.

The [null hypothesis](../../../../../../null-hypothesis.md) is $\beta_1=0$, leaving the [random slope](../../../../../../random-slope.md) variance free; the alternative permits a nonzero population stirring effect. The supplied test has $2(\ell_1-\ell_0)=7.9588$, one extra fixed coefficient, and approximate $\chi^2_1$ [p-value](../../../../../../p-value.md) $0.004786$. **Retain the fixed stirring-rate effect at 5%.** A mean-zero [random slope](../../../../../../random-slope.md) cannot substitute for an estimated nonzero population slope. The asymptotic calibration assumes regular nuisance covariance parameters and should be interpreted cautiously with only three furnaces; simulation can provide a better finite-sample calibration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

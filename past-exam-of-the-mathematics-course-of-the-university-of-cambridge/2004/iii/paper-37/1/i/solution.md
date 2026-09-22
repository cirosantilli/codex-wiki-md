<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $X$ be the $n\times p$ [design matrix](../../../../../../design-matrix.md) with row $x_i^T$, let $y=(y_i)$, and write $\mu_i(\beta)=\exp(x_i^T\beta)$. Independence gives the [Poisson regression](../../../../../../poisson-regression.md) [likelihood function](../../../../../../likelihood-function.md)

$$
L(\beta)=\prod_{i=1}^n\frac{e^{-\mu_i}\mu_i^{y_i}}{y_i!},\qquad
\ell(\beta)=\sum_i\{y_ix_i^T\beta-e^{x_i^T\beta}-\log(y_i!)\}.
$$

The [score function](../../../../../../informant-function.md) and negative [Hessian matrix](../../../../../../hessian-matrix.md) are

$$
\boxed{U(\beta)=X^T(y-\mu),\qquad I(\beta)=-\nabla^2\ell(\beta)=X^TWX,\quad W=\operatorname{diag}(\mu_i).}
$$

Because $EY_i=\mu_i$, the score has mean zero; independence and the [Poisson distribution](../../../../../../poisson-distribution.md) [variance](../../../../../../variance-split.md) give $\operatorname{Var}U=X^TWX$. Thus the observed and expected [Fisher information matrices](../../../../../../fisher-information-matrix.md) are the same here.

Assume $X$ has full column [matrix rank](../../../../../../matrix-rank.md) $p$. For a nonzero vector $a$, $a^TIa=\sum_i\mu_i(x_i^Ta)^2>0$. The [concavity of the Poisson regression likelihood](../../../../../../concavity-of-the-poisson-regression-likelihood.md) therefore makes any finite solution of $X^T(y-\widehat\mu)=0$ the unique [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md). If the design is rank deficient, parameters differing by a vector in $\ker X$ give the same distribution, so only identifiable combinations can be estimated. Full rank alone does not ensure a finite maximizer: for an intercept-only model with all observations zero, $\ell=-ne^\beta$ approaches its supremum as $\beta\to-\infty$. More generally, directions that decrease only fitted means attached to zero counts can produce boundary fits. A useful sufficient case for a finite fit is full rank with every count positive: each summand $y_i\eta_i-e^{\eta_i}$ tends to $-\infty$ in either tail, and some $|\eta_i|$ diverges whenever $\|\beta\|$ diverges.

For an interior fit, [Newton's method](../../../../../../newton-s-method-in-optimization.md) and [Fisher scoring](../../../../../../scoring-algorithm.md) give the same update:

$$
\beta^{(k+1)}=\beta^{(k)}+[X^TW^{(k)}X]^{-1}X^T(y-\mu^{(k)}).
$$

This is also [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). Define the working response $z_i=\eta_i+(y_i-\mu_i)/\mu_i$, with $\eta=X\beta^{(k)}$, and regress $z$ on $X$ using weights $W^{(k)}$:

$$
\beta^{(k+1)}=(X^TW^{(k)}X)^{-1}X^TW^{(k)}z.
$$

A numerical implementation solves these linear equations rather than explicitly forming the inverse, checks convergence of the score and [likelihood](../../../../../../likelihood-function.md), and can shorten a step when necessary.

Under the usual fixed-design regularity conditions, with growing information and no single observation dominating it, a score [Taylor expansion](../../../../../../taylor-expansion.md) about the true parameter gives

$$
\widehat\beta-\beta_0\approx I(\beta_0)^{-1}U(\beta_0),\qquad
\boxed{\widehat\beta\ \dot\sim\ N_p\big(\beta_0,I(\beta_0)^{-1}\big).}
$$

Estimate the [covariance matrix](../../../../../../covariance-matrix.md) by $[X^T\operatorname{diag}(\widehat\mu_i)X]^{-1}$; its diagonal square roots are the coefficient [standard errors](../../../../../../standard-error.md). This justifies large-sample [Wald confidence intervals](../../../../../../wald-confidence-interval.md) and [Wald tests](../../../../../../wald-test.md) for specified coefficients or contrasts. Finite-sample unbiasedness is not being asserted. A [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) compares nested fits through twice their maximized [log-likelihood](../../../../../../log-likelihood.md) difference. The [Poisson deviance](../../../../../../poisson-deviance.md) against the saturated fit is

$$
D=2\sum_i\left\{y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right\},
$$

with $0\log0=0$. Residual diagnostics and a check of [overdispersion](../../../../../../overdispersion.md) assess whether the assumed Poisson [variance](../../../../../../variance-split.md) is adequate; the [variance](../../../../../../variance-split.md) correction required when it is not is derived in the next part.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

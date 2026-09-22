<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [logistic regression](../../../../../../logistic-regression.md), set $\eta_i=x_i^{\mathsf T}\beta$ and $p_i=(1+e^{-\eta_i})^{-1}$. Its Bernoulli [log-likelihood](../../../../../../log-likelihood.md), [score function](../../../../../../informant-function.md) and [Fisher information](../../../../../../fisher-information-matrix.md) are

$$
\ell(\beta)=\sum_i\{y_i\eta_i-\log(1+e^{\eta_i})\},\qquad
U(\beta)=X^{\mathsf T}(y-p),\qquad
I(\beta)=X^{\mathsf T}WX,
$$

where $W=\operatorname{diag}\{p_i(1-p_i)\}$. Solve $U(\beta)=0$ by [Fisher scoring](../../../../../../scoring-algorithm.md) or [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). One scoring step is

$$
\boxed{\beta^{\rm new}=\beta+(X^{\mathsf T}WX)^{-1}X^{\mathsf T}(y-p)}.
$$

Equivalently regress the working response $z_i=\eta_i+(y_i-p_i)/[p_i(1-p_i)]$ on $X$ using weights $p_i(1-p_i)$. Iterate until the [likelihood](../../../../../../likelihood-function.md) and coefficients stabilize, with rank and convergence checks. [Separation in logistic regression](../../../../../../separation-in-logistic-regression.md) can prevent a finite maximum: if a predictor direction strictly separates the zeros and ones, moving indefinitely along it improves the [likelihood](../../../../../../likelihood-function.md) rather than producing a finite root.

Under the unrestricted model, each individual [probability](../../../../../../probability.md) is estimated independently as $\widehat p_i=y_i$. Every observed binary outcome then has [probability](../../../../../../probability.md) one, so, using boundary limits,

$$
\boxed{\max_{0\le p_i\le1}\ell(p_1,\ldots,p_n)=0}.
$$

The resulting [residual deviance](../../../../../../residual-deviance.md) is $D=-2\ell(\widehat\beta)$. It is a legitimate [likelihood](../../../../../../likelihood-function.md) contrast and can be used to compare fitted models. However, [individual Bernoulli deviance need not have a chi-squared calibration](../../../../../../individual-bernoulli-deviance-need-not-have-a-chi-squared-calibration.md): the saturated model has one boundary-valued parameter for each single observation, and its dimension grows with $n$. The fixed-dimensional regularity behind [Wilks theorem](../../../../../../wilks-theorem.md) does not justify a $\chi^2_{n-p}$ reference here.

For a concrete demonstration, let the true model contain only an intercept and have success [probability](../../../../../../probability.md) $1/2$. Its fitted [probability](../../../../../../probability.md) is $\bar y$, and

$$
\frac Dn=-2\{\bar y\log\bar y+(1-\bar y)\log(1-\bar y)\}
\longrightarrow2\log2,
$$

whereas a $\chi^2_{n-1}$ variable divided by $n$ converges to one. Thus treating the raw Bernoulli [residual deviance](../../../../../../residual-deviance.md) as an ordinary absolute goodness-of-fit statistic can reject a correct model systematically. In contrast, [deviance](../../../../../../exponential-family-deviance.md) differences between fixed-dimensional nested logistic models have their usual asymptotic chi-squared reference under the relevant regularity assumptions. For absolute fit use meaningful replicated covariate groups and [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md), or assess residual patterns and prediction on held-out data; a model-specific [parametric bootstrap](../../../../../../parametric-bootstrap.md) can calibrate a chosen statistic.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

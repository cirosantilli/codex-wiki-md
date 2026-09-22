<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the negative-binomial size $\theta>0$ held fixed, collect all mean-[independent](../../../../../../independent-random-variables.md) terms into $c(y_i,\theta)$. The cell [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell_i(\mu_i)=c(y_i,\theta)+y_i\log\mu_i-(y_i+\theta)\log(\mu_i+\theta).
$$

Its derivative is

$$
\ell_i'(\mu_i)=\frac{y_i}{\mu_i}-\frac{y_i+\theta}{\mu_i+\theta}
=\frac{\theta(y_i-\mu_i)}{\mu_i(\mu_i+\theta)}.
$$

For $y_i>0$ it is positive below $y_i$ and negative above $y_i$, so the saturated maximum is at $\mu_i=y_i$. For $y_i=0$, the maximum is the boundary limit $\mu_i\downarrow0$. Evaluating the saturated-minus-fitted [log-likelihood](../../../../../../log-likelihood.md) gives the [negative binomial deviance](../../../../../../negative-binomial-deviance.md)

$$
\boxed{D_n=2\sum_i y_i\log\frac{y_i}{e_i}
-2\sum_i(y_i+\theta)\log\frac{y_i+\theta}{e_i+\theta}}.
$$

All gamma-function and factorial terms cancel because the same known $\theta$ is used in both models. The zero-count logarithmic term is interpreted as zero; its remaining cell contribution is $2\theta\log(1+e_i/\theta)\ge0$. No intercept score cancellation is required for this formula, so it applies to the specified design whether or not its covariates include an intercept.

For completeness, the fitted coefficients obey the score equations of the [fixed-size negative binomial generalized linear model](../../../../../../fixed-size-negative-binomial-generalized-linear-model.md),

$$
\sum_i x_i\frac{\theta(y_i-e_i)}{\theta+e_i}=0,\qquad e_i=\exp(\widehat\beta^{\mathsf T}x_i).
$$

The logarithmic link is not the canonical link for this family, but it produces the requested positive means. As a check, when $\theta\to\infty$,

$$
(y_i+\theta)\log\frac{y_i+\theta}{e_i+\theta}\longrightarrow y_i-e_i,
$$

so the formula tends to the full [Poisson deviance](../../../../../../poisson-deviance.md), including the linear terms when an intercept-balance equation is unavailable. The size $\theta$ used here is the negative-binomial size parameter; it is distinct from the random-multiplier [variance](../../../../../../variance-split.md) denoted by the same letter in Question 4.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

`factor(day)` treats the nine days as categorical rather than imposing a numerical time trend. `rep(400,27)` supplies the number of trials for every dish, and `prop` is the observed surviving proportion. The contrast setting uses [treatment coding](../../../../../../treatment-coding.md) with day 1 as reference; the ordered-factor [polynomial](../../../../../../polynomial-split.md) option is unused. Supplying these proportions to `glm` with the binomial family and weights $400$ gives precisely the [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) [likelihood](../../../../../../likelihood-function.md) for the counts. The weights represent trial counts, not additional independent dish observations. The binomial family's default link is the [logit link](../../../../../../logit.md) and its dispersion is fixed at $1$.

Let $Y_{ij}$ be survivors in dish $j=1,2,3$ on day $i=1,\ldots,9$. Both fitted models assume independent $Y_{ij}\sim\operatorname{Bin}(400,p_i)$. Model 1 specifies

$$
\log\frac{p_i}{1-p_i}=\mu\qquad\text{for every day},
$$

so it has one common probability and one fitted coefficient. Its estimated probability is the total surviving count divided by the total trial count, $\widehat p=3539/10800\simeq0.327685$.

Model 2 specifies

$$
\log\frac{p_i}{1-p_i}=\mu+\alpha_i,\qquad\alpha_1=0.
$$

It has nine coefficients and allows a separate probability for each day, while retaining a common probability for the three dishes within that day. The MLEs are the day totals divided by $1200$. In day order they are

$$
\widehat p_i=(0.49000,\ 0.28000,\ 0.18417,\ 0.31667,\ 0.36583,\ 0.31500,\ 0.46833,\ 0.21167,\ 0.31750).
$$

The intercept is the first day's logit, and each other coefficient is its day's logit minus that reference. These are additive effects on log odds, not additive changes in survival probability.

The [analysis of deviance](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) adds the eight day indicators after an intercept-only model. Its residual [deviance](../../../../../../exponential-family-deviance.md) compares a fitted model with the [saturated statistical model](../../../../../../saturated-statistical-model.md) assigning one separate probability to each of the $27$ dishes. For fitted dish probabilities $\widehat p_{ij}$, the [binomial deviance](../../../../../../binomial-deviance.md) is

$$
D=2\sum_{i,j}\left\{Y_{ij}\log\frac{Y_{ij}}{400\widehat p_{ij}}+(400-Y_{ij})\log\frac{400-Y_{ij}}{400(1-\widehat p_{ij})}\right\}.
$$

The binomial scale is one, so this is also [scaled deviance](../../../../../../scaled-deviance.md). The reported decrease measures the extra fit provided by day. There are $27$ observational units for these residual [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md), not $10800$ separately fitted Bernoulli responses.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="section-d/d13/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Bayes' theorem](../../../../../../bayes-theorem.md) updates prior knowledge using the [likelihood](../../../../../../likelihood-function.md) of new observations. For alternative hypotheses $H_j$,

$$
\boxed{P(H_j\mid D)=\frac{P(D\mid H_j)P(H_j)}{\sum_kP(D\mid H_k)P(H_k)}.}
$$

The prior $P(H_j)$ describes information before the data $D$; $P(D\mid H_j)$ is the sampling [likelihood](../../../../../../likelihood-function.md), and the posterior $P(H_j\mid D)$ describes the updated probabilities. Posterior odds equal prior odds times the [likelihood](../../../../../../likelihood-function.md) ratio. A [likelihood](../../../../../../likelihood-function.md) is a [probability](../../../../../../probability.md) model for data at specified parameters, not automatically a normalized [probability](../../../../../../probability.md) distribution over those parameters.

For a continuous parameter $\theta$, the same rule uses densities: $\pi(\theta\mid D)=L(D\mid\theta)\pi(\theta)/\int L(D\mid u)\pi(u)du$. Priors can encode positivity, physical limits, previous independent measurements or calibration knowledge. Their parameterization matters: a density uniform in a rate is not uniform in its logarithm. Proper priors make model evidences well defined; an arbitrary normalization in an improper prior is especially problematic for comparing models.

A counting example uses [Poisson-gamma conjugacy](../../../../../../poisson-gamma-conjugacy.md). If a detector registers $K$ events in exposure $t$ with constant rate $\lambda$, $L\propto\lambda^Ke^{-t\lambda}$. A gamma prior with shape $\alpha$ and rate parameter $\beta$, $\pi(\lambda)\propto\lambda^{\alpha-1}e^{-\beta\lambda}$, gives

$$
\boxed{\lambda\mid K\sim\operatorname{Gamma}(\alpha+K,\beta+t),\qquad \mathbb E[\lambda\mid K]=\frac{\alpha+K}{\beta+t}.}
$$

The [posterior mean](../../../../../../posterior-mean.md) combines the prior rate $\alpha/\beta$ with the observed rate $K/t$, weighted by the prior and actual exposures. The parameters must use a consistent shape-rate convention. Small counts can leave substantial prior sensitivity; abundant informative data usually reduce it for regular identifiable models.

Independent old data can become the prior for a new experiment, giving the same result as joint updating under a consistent model. The new data must not also have been used to construct that prior, or the evidence is counted twice. A [credible interval](../../../../../../credible-interval.md) has a specified posterior [probability](../../../../../../probability.md) under the chosen model and prior; this interpretation differs from repeated-sampling coverage of a [confidence interval](../../../../../../confidence-interval.md). Predictions for a future observation average its sampling distribution over the posterior, incorporating parameter uncertainty. Prior sensitivity checks and a defensible [likelihood](../../../../../../likelihood-function.md) are therefore part of the inference, rather than [Bayes' theorem](../../../../../../bayes-theorem.md) itself supplying missing physical knowledge.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

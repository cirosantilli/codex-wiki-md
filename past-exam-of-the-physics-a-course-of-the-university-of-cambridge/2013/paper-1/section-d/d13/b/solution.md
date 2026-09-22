<h1 id="section-d/d13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [likelihood](../../../../../../likelihood-function.md) is $L(\theta;d)=p(d\mid\theta)$ considered as a function of parameters at the observed data. It is not itself a probability distribution over $\theta$. [Bayes' theorem](../../../../../../bayes-theorem.md) gives

$$
\boxed{p(\theta\mid d)=\frac{p(d\mid\theta)\pi(\theta)}{\int p(d\mid\vartheta)\pi(\vartheta)\,d\vartheta}}.
$$

The [prior](../../../../../../prior-probability.md) represents parameter information before these data; the denominator normalizes the [posterior](../../../../../../bayesian-posterior.md) and can compare fully specified models with compatible [prior](../../../../../../prior-probability.md) assumptions. Detector response, backgrounds, dependence and selection must be included in the data model.

For independent measurements $x_i\sim N(\theta,\sigma_i^2)$ with known errors, $\log L=\mathrm{constant}-\tfrac12\sum_i(x_i-\theta)^2/\sigma_i^2$. Maximum [likelihood](../../../../../../likelihood-function.md) minimizes this [chi-squared](../../../../../../chi-squared-distribution.md) and gives $\widehat\theta=\sum_iw_ix_i/\sum_iw_i$, $w_i=\sigma_i^{-2}$. A [Gaussian](../../../../../../normal-distribution.md) [prior](../../../../../../prior-probability.md) $N(\mu_0,s_0^2)$ instead yields

$$
\boxed{s_{\rm post}^2=\frac1{\sum_iw_i+s_0^{-2}},\qquad
\mu_{\rm post}=s_{\rm post}^2\left(\sum_iw_ix_i+\frac{\mu_0}{s_0^2}\right)}.
$$

This explicitly combines data and [prior](../../../../../../prior-probability.md) precision, approaching the [weighted mean](../../../../../../weighted-arithmetic-mean.md) when [prior](../../../../../../prior-probability.md) information is weak. Unknown [calibration](../../../../../../calibration-differential-geometry.md) parameters should be jointly inferred and marginalized, not silently fixed. [posterior](../../../../../../bayesian-posterior.md) intervals are conditional on the assumed model and [prior](../../../../../../prior-probability.md); [posterior predictive checks](../../../../../../posterior-predictive-check.md) and sensitivity to plausible [priors](../../../../../../prior-probability.md) help expose poor fits and weakly identified parameters. The maximum-likelihood estimate and a Bayesian [posterior](../../../../../../bayesian-posterior.md) answer different inferential questions even when their numerical centres agree.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2013](../../../../split.md)
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

<h1 id="section-d/d12/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Bayes' theorem](../../../../../../bayes-theorem.md) updates a parameter distribution using measured data:

$$
\boxed{p(\theta\mid D)=\frac{p(D\mid\theta)p(\theta)}{\int p(D\mid\theta')p(\theta')\,d\theta'}}.
$$

The [likelihood](../../../../../../likelihood-function.md) describes the measurement process, the [prior distribution](../../../../../../prior-probability.md) encodes information before the present data, and the denominator normalizes the [posterior distribution](../../../../../../bayesian-posterior.md). Include instrumental [noise](../../../../../../noise-signal-processing.md) and known selection effects in the [likelihood](../../../../../../likelihood-function.md). [nuisance parameters](../../../../../../nuisance-parameter.md), such as an uncertain background, should be jointly inferred and marginalized, rather than silently fixed.

For $n$ independent readings with a [Gaussian distribution](../../../../../../normal-distribution.md) with known common [variance](../../../../../../variance-split.md) $\sigma^2$ and [prior distribution](../../../../../../prior-probability.md) $\theta\sim N(\mu_0,\tau_0^2)$, completing the square gives

$$
\tau_n^{-2}=\tau_0^{-2}+n\sigma^{-2},\qquad
\mu_n=\tau_n^2\big(\mu_0\tau_0^{-2}+n\bar x\,\sigma^{-2}\big).
$$

The [posterior distribution](../../../../../../bayesian-posterior.md) is $N(\mu_n,\tau_n^2)$: [prior distribution](../../../../../../prior-probability.md) and data contribute in proportion to precision. A broad [prior distribution](../../../../../../prior-probability.md) recovers the usual estimate $\bar x$ with [standard deviation](../../../../../../standard-deviation.md) $\sigma/\sqrt n$. Report a [posterior distribution](../../../../../../bayesian-posterior.md) estimate and [credible interval](../../../../../../credible-interval.md), specify the [prior distribution](../../../../../../prior-probability.md), and examine sensitivity when the data are weak. A [credible interval](../../../../../../credible-interval.md) is a [posterior distribution](../../../../../../bayesian-posterior.md) [probability](../../../../../../probability.md) statement about the parameter conditional on the model; it is not defined by the repeated-sampling coverage of a [confidence interval](../../../../../../confidence-interval.md).

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2011](../../../../split.md)
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

<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $s=\sum_i x_i$. The [Bernoulli distribution](../../../../../bernoulli-distribution.md) [likelihood function](../../../../../likelihood-function.md) is $\theta^s(1-\theta)^{n-s}$. Multiplication by the [beta distribution](../../../../../beta-distribution.md) [prior density](../../../../../prior-density.md) and [Bayes' theorem](../../../../../bayes-theorem.md) give

$$
\pi(\theta\mid x)\propto\theta^{a+s-1}(1-\theta)^{b+n-s-1},\qquad0<\theta<1.
$$

Recognizing the normalized [beta distribution](../../../../../beta-distribution.md),

$$
\boxed{\theta\mid x\sim\operatorname{Beta}(a+s,b+n-s),\qquad
\pi(\theta\mid x)=\frac{\theta^{a+s-1}(1-\theta)^{b+n-s-1}}{B(a+s,b+n-s)}.}
$$

This is [Beta-binomial conjugacy](../../../../../beta-binomial-conjugacy.md); the same update applies whether the data are recorded as the individual [Bernoulli trials](../../../../../bernoulli-trial.md) or their success count.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

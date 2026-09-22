<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [exponential distribution](../../../../../exponential-distribution.md) prior has rate $\lambda=1/3$ and support $\mu\geq0$, so its [prior density](../../../../../prior-density.md) is $(1/3)e^{-\mu/3}\mathbf1_{\{\mu\geq0\}}$. By [Bayes' theorem](../../../../../bayes-theorem.md),

$$
\boxed{p(\mu\mid x)=C\exp\!\left[-\frac12\sum_i(x_i-\mu)^2-\frac\mu3\right]
\mathbf1_{\{\mu\geq0\}}},
$$

where $C$ is a [normalizing constant](../../../../../normalizing-constant.md) independent of $\mu$.

Completing the square gives a useful exact reference for the numerical sampling. Put

$$
m=\bar x-\frac1{3n},\qquad s=\frac1{\sqrt n}.
$$

Then this [normal mean posterior with an exponential prior](../../../../../normal-mean-posterior-with-an-exponential-prior.md) is a [normal distribution](../../../../../normal-distribution.md) with location $m$ and [variance](../../../../../variance-split.md) $s^2$, truncated below at zero. With $\phi$ the [standard normal distribution](../../../../../standard-normal-distribution.md) density and $\Phi$ its [cumulative distribution function](../../../../../cumulative-distribution-function.md),

$$
\boxed{p(\mu\mid x)=\frac{\phi((\mu-m)/s)}{s\Phi(m/s)}\mathbf1_{\{\mu\geq0\}}}.
$$

The exponential rate is $1/3$, not three; the [prior mean](../../../../../prior-mean.md) is three. The support restriction must be retained in both the formula and the sampler.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

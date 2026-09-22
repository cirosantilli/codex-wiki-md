# Laplace distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_distribution)

The [Laplace distribution](laplace-distribution.md), also called the [double exponential distribution](laplace-distribution.md), is a [location-scale family](location-scale-family.md) with [probability density function](probability-density-function.md)

$$
f(x;\mu,b)=\frac1{2b}\exp\!\left(-\frac{|x-\mu|}{b}\right),\qquad x\in\mathbb R,\quad\mu\in\mathbb R,\quad b>0.
$$

The location $\mu$ is its [mean](expected-value-split.md), [median](median.md) and [mode](mode-statistics.md); $b$ controls its spread. In the centred rate convention, the same law has $\mu=0$ and $\theta=1/b>0$, giving $f(x)=\theta e^{-\theta|x|}/2$. Keeping track of whether a parameter is a scale or its reciprocal prevents reversing the effect of increasing it. [NIST and SEMATECH e-Handbook of Statistical Methods; NIST/SEMATECH e-Handbook, Section 1.3.6.6.12, Probability Density Function and Common Statistics; NIST denotes the scale by beta](nist-and-sematech-e-handbook-of-statistical-methods/1-3-6-6-12-double-exponential-distribution.md)

The two halves of the [probability density function](probability-density-function.md) are reflected [exponential decay](exponential-decay.md) curves, each with total [probability](probability.md) $1/2$. Their meeting point has a sharp corner: the left and right [derivatives](derivative.md) are $1/(2b^2)$ and $-1/(2b^2)$. This finite peak is not a positive [probability mass](probability-mass.md) at $\mu$. Indeed

$$
\mathbb P(|X-\mu|\leq\varepsilon)=1-e^{-\varepsilon/b}\longrightarrow0\qquad(\varepsilon\downarrow0),
$$

so $\mathbb P(X=\mu)=0$, just as for any [absolutely continuous probability distribution](absolutely-continuous-probability-distribution.md).

<a id="image-laplace-and-normal-densities-and-two-sided-tails-with-the-same-mean-and-variance"></a>
![](laplace-density-and-log-tail-comparison.png)

**[Figure 9](#image-laplace-and-normal-densities-and-two-sided-tails-with-the-same-mean-and-variance). Laplace and normal densities and two-sided tails with the same mean and variance**.

The figure compares a [Laplace distribution](laplace-distribution.md) with $\mu=0$, $b=1$ against a [normal distribution](normal-distribution.md) with [mean](expected-value-split.md) zero and [standard deviation](standard-deviation.md) $\sigma=\sqrt2$: both have [variance](variance-split.md) 2. The right panel uses a [logarithmic scale](logarithmic-scale.md) for the two-sided tail [probability](probability.md) $\mathbb P(|X|>r)$. Its straight [Laplace distribution](laplace-distribution.md) curve comes from $e^{-r}$; the [normal distribution](normal-distribution.md) tail falls faster. Thus values far from the center can be more plausible under a [Laplace distribution](laplace-distribution.md) even after matching the [variance](variance-split.md). These are theoretical curves, not measured frequencies. The tails still have [exponential decay](exponential-decay.md); this is not a [heavy-tailed distribution](heavy-tailed-distribution.md) in the convention requiring every positive [exponential moment](exponential-moment.md) to diverge.

Integrating either half of the [probability density function](probability-density-function.md) gives the [cumulative distribution function](cumulative-distribution-function.md)

$$
F(x)=\begin{cases}
\tfrac12e^{(x-\mu)/b},&x<\mu,\\
1-\tfrac12e^{-(x-\mu)/b},&x\geq\mu.
\end{cases}
$$

In particular $F(\mu)=1/2$. The basic [moments](moment.md) are

$$
\mathbb E[X]=\mu,\qquad \mathbb E|X-\mu|=b,\qquad \operatorname{Var}(X)=2b^2,\qquad \operatorname{SD}(X)=\sqrt2\,b.
$$

Thus the scale is the [expected value](expected-value-split.md) of the absolute distance from the center, and is not the [standard deviation](standard-deviation.md). [NIST and SEMATECH e-Handbook of Statistical Methods; NIST/SEMATECH e-Handbook, Section 1.3.6.6.12, Cumulative Distribution Function and Common Statistics; rescale the standard form by x=mu+bz](nist-and-sematech-e-handbook-of-statistical-methods/1-3-6-6-12-double-exponential-distribution.md) A short way to obtain the [moments](moment.md) is to note that $R=|X-\mu|$ has an [exponential distribution](exponential-distribution.md) with rate $1/b$: $\mathbb P(R>r)=e^{-r/b}$ for $r\geq0$. Integrating gives $\mathbb E R=b$ and $\mathbb E R^2=2b^2$; the [symmetric distribution](symmetric-distribution.md) gives the centered first [moment](moment.md) zero.

**Table of contents**

- [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)
  - [Laplace median robustness example](laplace-median-robustness-example.md)
- [Laplace prior for sparse images](laplace-prior-for-sparse-images.md)
- [Laplace regression](laplace-regression.md)

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (26)

- [Laplace distribution](laplace-distribution.md)
- [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)
- [Laplace median robustness example](laplace-median-robustness-example.md)
- [Laplace prior for sparse images](laplace-prior-for-sparse-images.md)
- [Laplace ratio-of-uniforms envelope](laplace-ratio-of-uniforms-envelope.md)
- [Lévy measure of a symmetric Laplace time-one law](levy-measure-of-a-symmetric-laplace-time-one-law.md)
- [Moreau smoothing of a negative log-density](moreau-smoothing-of-a-negative-log-density.md)
- [Most powerful test for a Laplace location shift](most-powerful-test-for-a-laplace-location-shift.md)
- [Pareto distribution](pareto-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/21h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/5i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/26k/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/4/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-350/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/3/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/5j/solution.md)
- [Rayleigh-normal scale mixture](rayleigh-normal-scale-mixture.md)
- [Saddlepoint density of a Laplace sample mean](saddlepoint-density-of-a-laplace-sample-mean.md)
- [Self-convolution of a bilateral exponential](self-convolution-of-a-bilateral-exponential.md)
- [Squared Rayleigh radius](squared-rayleigh-radius.md)

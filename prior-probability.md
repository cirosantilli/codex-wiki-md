# Prior probability

↑ **Parent:** [Bayesian statistics](bayesian-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prior_probability)

[Prior probability](prior-probability.md) describes uncertainty before the current observations are incorporated. For a [statistical parameter](statistical-parameter.md) $\Theta$, a [prior distribution](prior-probability.md) assigns [probabilities](probability.md) to its possible ranges, conditional on background information and a [statistical model](statistical-model-split.md). A continuous [prior density](prior-density.md) $\pi(\theta)$ specifies these probabilities through [integration](integral.md):

$$
\mathbb P(\Theta\in A)=\int_A\pi(\theta)\,d\theta,\qquad \pi(\theta)\geq0,\qquad \int\pi(\theta)\,d\theta=1.
$$

Here the [probability density function](probability-density-function.md) is relative to [Lebesgue measure](lebesgue-measure.md) $d\theta$; a discrete [prior distribution](prior-probability.md) instead uses a [probability mass function](probability-mass-function.md) and sums. Density at one point is not the [probability](probability.md) of that point. A nonnegative kernel with infinite total mass is an [improper prior](improper-prior.md), whose use requires a separate check of [posterior propriety](posterior-propriety.md).

For the coin model in [Bayesian statistics](bayesian-statistics.md), the [beta distribution](beta-distribution.md) $\operatorname{Beta}(2,2)$ has [prior density](prior-density.md) $\pi(\theta)=6\theta(1-\theta)$ on $[0,1]$. Its [mean](expected-value.md) is $1/2$ and its [variance](variance-split.md) is $1/20$. It favors moderate heads probabilities without ruling out values near zero or one. For example,

$$
\mathbb P(\Theta>3/4)=\int_{3/4}^1 6\theta(1-\theta)\,d\theta=\frac5{32}=0.15625.
$$

The prior curve in [Bayesian posterior](bayesian-posterior.md) makes this preference visible; [moment matching for a beta prior](moment-matching-for-a-beta-prior.md) explains how to choose a [beta distribution](beta-distribution.md) from a desired [mean](expected-value.md) and [variance](variance-split.md).

A [prior distribution](prior-probability.md) lets earlier evidence or elicited knowledge contribute to [statistical inference](statistical-inference-split.md) when the current [sample size](sample-size.md) is limited. It also exposes assumptions that can be checked by [prior elicitation](prior-elicitation.md) and a [prior predictive check](prior-predictive-check.md). Before the same eight heads and two tails, a [uniform prior](uniform-prior.md) $\operatorname{Beta}(1,1)$ would give [posterior mean](posterior-mean.md) $9/12=3/4$, compared with $5/7$ under $\operatorname{Beta}(2,2)$: the observations do not uniquely determine a [Bayesian posterior](bayesian-posterior.md). Even a [uniform prior](uniform-prior.md) makes a choice of parameter coordinates; its child article explains why changing coordinates can destroy uniformity.

**Table of contents**

- [Prior elicitation](prior-elicitation.md)
- [Prior odds](prior-odds.md)
- [Prior density](prior-density.md)
- [Continuous spike-and-slab prior](continuous-spike-and-slab-prior.md)
- [Uniform prior](uniform-prior.md)

## ↑ Ancestors (6)

1. [Bayesian statistics](bayesian-statistics.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Bayes' theorem](bayes-theorem.md)
- [Chernoff information](chernoff-information.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
- [Finite-sample Chernoff error bound](finite-sample-chernoff-error-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323/1/i/solution.md)
- [Prior odds](prior-odds.md)
- [Prior probability](prior-probability.md)

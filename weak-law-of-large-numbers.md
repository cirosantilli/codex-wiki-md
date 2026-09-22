# Weak law of large numbers

↑ **Parent:** [Convergence in probability](convergence-in-probability.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_law_of_large_numbers)

Let $X_1,X_2,\ldots$ be real [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with $\mathbb E|X_1|<\infty$ and [expected value](expected-value.md) $\mu=\mathbb E[X_1]$. The [weak law of large numbers](weak-law-of-large-numbers.md) states that their [sample mean](sample-mean.md) has [convergence in probability](convergence-in-probability.md) to $\mu$: for every fixed $\varepsilon>0$,

$$
\mathbb P\left(\left|\overline X_n-\mu\right|\geq\varepsilon\right)\longrightarrow0,
\qquad
\overline X_n=\frac1n\sum_{j=1}^nX_j.
$$

Thus a large sample is unlikely to give an average with a specified fixed-size error. The [strong law of large numbers](strong-law-of-large-numbers.md) makes the stronger statement of [almost sure convergence](almost-sure-convergence.md) along an entire sequence. Under the displayed assumptions both laws apply; their names distinguish the conclusions, not two competing predictions.

When the [variance](variance-split.md) $\sigma^2$ is finite, [variance additivity for independent random variables](variance-additivity-for-independent-random-variables.md) gives $\operatorname{Var}(\overline X_n)=\sigma^2/n$. The [Chebyshev inequality](chebyshev-s-inequality.md) immediately supplies a useful quantitative form and a brief proof:

$$
\mathbb P\left(\left|\overline X_n-\mu\right|\geq\varepsilon\right)
\leq\min\left(1,\frac{\sigma^2}{n\varepsilon^2}\right).
$$

For [independent](independent-random-variables.md) trials with a [Bernoulli distribution](bernoulli-distribution.md) of parameter $p=0.2$, the [expected value](expected-value.md) is $0.2$ and the [variance](variance-split.md) is $0.16$. At $n=1000$, the chance of an error of at least $0.1$ is therefore at most $0.016$. The exact [binomial distribution](binomial-distribution.md) gives a much smaller [probability](probability.md), as the figure under the [strong law of large numbers](strong-law-of-large-numbers.md) shows. The bound is conservative, but it is valid for every sample size under these assumptions and does not require a [normal approximation](normal-approximation.md).

The [weak law of large numbers](weak-law-of-large-numbers.md) addresses a fixed tolerance $\varepsilon$. The [central limit theorem](central-limit-theorem.md) instead resolves errors on the shrinking scale $\sigma/\sqrt n$ and gives their approximate [normal distribution](normal-distribution.md). In particular, the [weak law of large numbers](weak-law-of-large-numbers.md) alone supplies neither a bell-shaped error law nor a universal rate of approach. For example, a [Pareto distribution](pareto-distribution.md) with minimum one and shape $3/2$ has [expected value](expected-value.md) three but infinite [variance](variance-split.md): both the [weak law of large numbers](weak-law-of-large-numbers.md) and [strong law of large numbers](strong-law-of-large-numbers.md) apply, while the finite-[variance](variance-split.md) statement of the [central limit theorem](central-limit-theorem.md) does not.

**Table of contents**

- [Weak law without an absolute first moment](weak-law-without-an-absolute-first-moment.md)
- [Weak law forces a characteristic-function derivative](weak-law-forces-a-characteristic-function-derivative.md)
- [Uniform law of large numbers](uniform-law-of-large-numbers.md)
  - [Pointwise separable function class](pointwise-separable-function-class.md)
  - [Bracketing of a function class](bracketing-of-a-function-class.md)
    - [Integrable envelope of a function class](integrable-envelope-of-a-function-class.md)
    - [Uniform strong law from finite L1 bracketing](uniform-strong-law-from-finite-l1-bracketing.md)
      - [Uniform strong law on a compact parameter set](uniform-strong-law-on-a-compact-parameter-set.md)
  - [Glivenko-Cantelli theorem](glivenko-cantelli-theorem.md)
    - [Quantile proof of the Glivenko-Cantelli theorem](quantile-proof-of-the-glivenko-cantelli-theorem.md)

## ↑ Ancestors (7)

1. [Convergence in probability](convergence-in-probability.md)
2. [Convergence of random variables](convergence-of-random-variables-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (56)

- [Cauchy sample mean has an unchanged distribution](cauchy-sample-mean-has-an-unchanged-distribution.md)
- [Central limit theorem](central-limit-theorem.md)
- [Characteristic-function derivative under an absolute first moment](characteristic-function-derivative-under-an-absolute-first-moment.md)
- [Chebyshev's inequality](chebyshev-s-inequality.md)
- [Convergence of random variables](convergence-of-random-variables-split.md)
- [Law of large numbers](law-of-large-numbers.md)
- [Pafnuty Chebyshev](pafnuty-chebyshev.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-2/12f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-34/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/29k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-215/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/2/i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/2/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-221/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-224/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-224/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-225/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-205/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-225/4/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-225/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-225/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-210/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-224/2/a/solution.md)
- [Quantum typical subspace](quantum-typical-subspace.md)
- [Realized absolute covariation](realized-absolute-covariation.md)
- [Strong law of large numbers](strong-law-of-large-numbers.md)
- [Tripartite Schmidt projection entanglement concentration](tripartite-schmidt-projection-entanglement-concentration.md)
- [Typical sequence theorem](typical-sequence-theorem.md)
- [Typical subspace theorem](typical-subspace-theorem.md)
- [Weak law of large numbers](weak-law-of-large-numbers.md)
- [Weak law without an absolute first moment](weak-law-without-an-absolute-first-moment.md)
- [Weakly typical sequence](weakly-typical-sequence.md)
- [Worst-case correction guarantee from the Gilbert–Varshamov bound](worst-case-correction-guarantee-from-the-gilbert-varshamov-bound.md)

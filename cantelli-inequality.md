# Cantelli inequality

↑ **Parent:** [Chebyshev's inequality](chebyshev-s-inequality.md)

[Cantelli's inequality](cantelli-inequality.md) uses a [mean](expected-value-split.md) and [variance](variance-split.md) to control deviations in one specified direction. For a real [random variable](random-variable-split.md) $X$ with [expected value](expected-value-split.md) $\mu$, finite [variance](variance-split.md) $\sigma^2$, and $a>0$,

$$
\boxed{\mathbb P(X-\mu\geq a)\leq\frac{\sigma^2}{\sigma^2+a^2}.}
$$

Applying the same statement to $-X$ gives the lower [tail probability](tail-probability.md) bound $\mathbb P(X-\mu\leq-a)\leq\sigma^2/(\sigma^2+a^2)$. No [independence](independent-random-variables.md) or particular [probability distribution](probability-distribution-split.md) is required. If $\sigma^2=0$, the [random variable](random-variable-split.md) equals $\mu$ [almost surely](almost-sure-convergence.md) and both positive-threshold [tail probabilities](tail-probability.md) are zero.

For [variance](variance-split.md) one and a threshold two above the [mean](expected-value-split.md), **the upper-tail [probability](probability.md) is at most $1/5$**. Applying the two-sided [Chebyshev's inequality](chebyshev-s-inequality.md) to contain that upper [event](event.md) would give the weaker bound $1/4$. For the [standard normal distribution](standard-normal-distribution.md), the actual upper [tail probability](tail-probability.md) at two is about $0.0227501$, much smaller than either bound. Yet the two-point [probability distribution](probability-distribution-split.md) in [equality in Cantelli's inequality](equality-in-cantelli-s-inequality.md) attains $1/5$, showing why the smaller Gaussian value cannot be promised from these two [moments](moment.md) alone.

<a id="image-cantelli-s-inequality-sharpens-a-variance-only-upper-tail-bound-and-is-exact-for-a-two-point-probability-distribution"></a>
![](cantelli-one-sided-bound-and-extremizer.png)

**[Figure 3](#image-cantelli-s-inequality-sharpens-a-variance-only-upper-tail-bound-and-is-exact-for-a-two-point-probability-distribution). Cantelli's inequality sharpens a variance-only upper-tail bound and is exact for a two-point probability distribution**. Left: actual upper [tail probabilities](tail-probability.md) for the [standard normal distribution](standard-normal-distribution.md) are compared with [Cantelli's inequality](cantelli-inequality.md) and the capped two-sided [Chebyshev's inequality](chebyshev-s-inequality.md) used as an upper-tail bound. Right: masses $4/5$ at $-1/2$ and $1/5$ at two have [mean](expected-value-split.md) zero and [variance](variance-split.md) one. The upper mass is included by the non-strict threshold $X\geq2$. These are specified mathematical models, not observations.

A short explanation is to centre $Y=X-\mu$ and choose a nonnegative shift $b$. On $Y\geq a$, the square $(Y+b)^2$ is at least $(a+b)^2$, so [Markov's inequality](markov-s-inequality.md) gives

$$
\mathbb P(Y\geq a)\leq\frac{\mathbb E(Y+b)^2}{(a+b)^2}=\frac{\sigma^2+b^2}{(a+b)^2}.
$$

The best shift is $b=\sigma^2/a$, giving the displayed bound. Choosing the shift before squaring exploits the direction of the deviation; squaring the unshifted [random variable](random-variable-split.md) treats both directions together. This shifted-square proof is also the strategy requested in the University of Utah's 2005 qualifying problem on [Cantelli's inequality](cantelli-inequality.md). [University of Utah Mathematics, 2005 question 4: shifted-square Cantelli bound](https://quals.math.utah.edu/topics/borel-cantelli-lemmas/).

The one-sided improvement should be used for a one-sided question. Adding upper and lower bounds by the [union bound](boole-s-inequality.md) gives $2\sigma^2/(\sigma^2+a^2)$ for $|X-\mu|\geq a$. When $a\geq\sigma>0$, that is at least the [Chebyshev's inequality](chebyshev-s-inequality.md) bound $\sigma^2/a^2$; when $a<\sigma$, both two-sided expressions exceed one and must be capped. The separate one-sided bounds generally cannot be attained simultaneously by the same [probability distribution](probability-distribution-split.md).

**Table of contents**

- [Equality in Cantelli's inequality](equality-in-cantelli-s-inequality.md)

## ↑ Ancestors (7)

1. [Chebyshev's inequality](chebyshev-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [One-sided maximal inequality for a centered square-integrable martingale](one-sided-maximal-inequality-for-a-centered-square-integrable-martingale.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/11f/solution.md)

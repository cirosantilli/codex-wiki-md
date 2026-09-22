# Covariance of draws without replacement

↑ **Parent:** [Sampling without replacement](sampling-without-replacement.md)

Draw two distinct positions uniformly from a fixed population $z_1,\ldots,z_N$ with $N>1$. Let $\mu=N^{-1}\sum_i z_i$ and $\sigma_N^2=N^{-1}\sum_i(z_i-\mu)^2$. Each draw has [expected value](expected-value-split.md) $\mu$, while

$$
\mathbb E[Z_1Z_2]=\frac{(\sum_i z_i)^2-\sum_i z_i^2}{N(N-1)}=\mu^2-\frac{\sigma_N^2}{N-1}.
$$

Subtracting the product of the [expected values](expected-value-split.md) proves the [covariance](covariance.md) formula and explains the [finite population correction](finite-population-correction.md). If the sampled values are coin biases and the actual tosses are [conditionally independent](conditional-independence.md) given those biases, the [law of total covariance](law-of-total-covariance.md) gives the same [covariance](covariance.md) for their head [indicator random variables](indicator-random-variable.md).

## ↑ Ancestors (7)

1. [Sampling without replacement](sampling-without-replacement.md)
2. [Probability sampling](probability-sampling.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/7/b/i/solution.md)

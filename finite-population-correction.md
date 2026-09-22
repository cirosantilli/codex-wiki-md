# Finite population correction

↑ **Parent:** [Hypergeometric distribution](hypergeometric-distribution.md)

For uniform [sampling without replacement](sampling-without-replacement.md) from a population of $n>1$ objects, the [finite population correction](finite-population-correction.md) accounts for the reduced spread caused by drawing distinct objects. For the marked-object count $K$ in a [hypergeometric distribution](hypergeometric-distribution.md), put $p=c/n$. Then

$$
\mathbb E K=rp,\qquad
\operatorname{Var}(K)=rp(1-p)\frac{n-r}{n-1}.
$$

Relative to the corresponding [binomial distribution](binomial-distribution.md), the [variance](variance-split.md) is multiplied by $f^2=(n-r)/(n-1)$ and the [standard deviation](standard-deviation.md) by $f$. The square-root convention for the correction is used in Philip Stark's discussion of sample sums.[Stark, SticiGui, Standard Error: sample sums without replacement](https://www.stat.berkeley.edu/~stark/SticiGui/Text/standardError.htm)

The factor has a direct interpretation. For $r=1$, replacement makes no difference and $f=1$. For $r=n$, the entire population is observed and the marked count is exactly $c$, so $f=0$. In the ten-object, five-draw example, $f^2=5/9$ and $(6/5)(5/9)=2/3$. The exceptional population size $n=1$ is deterministic and should be handled directly rather than inserting it into a zero denominator.

A short explanation uses an [indicator random variable](indicator-random-variable.md) $I_j$ for a marked object at draw $j$. Each has [expected value](expected-value-split.md) $p$ and [variance](variance-split.md) $p(1-p)$. For distinct draw positions $i,j$,

$$
\mathbb E[I_iI_j]=\frac{c(c-1)}{n(n-1)},\qquad
\operatorname{Cov}(I_i,I_j)=-\frac{p(1-p)}{n-1}.
$$

Since $K=\sum_{j=1}^r I_j$, the [variance of a sum](variance-of-a-sum.md) includes $r$ individual terms and $r(r-1)$ ordered [covariance](covariance.md) terms, giving the displayed correction. [Linearity of expectation](linearity-of-expectation.md) still gives $rp$ despite this dependence.

For arbitrary fixed real population values, use $N>1$ for population size and $1\leq n\leq N$ for [sample size](sample-size.md). Write the [finite population mean](finite-population-mean.md) $\bar Y=N^{-1}\sum_i y_i$, the [finite population variance](finite-population-variance.md) $S^2=(N-1)^{-1}\sum_i(y_i-\bar Y)^2$ and $\sigma_N^2=N^{-1}\sum_i(y_i-\bar Y)^2$. Under [simple random sampling without replacement](simple-random-sampling.md), the [sample mean](sample-mean.md) satisfies

$$
\operatorname{Var}(\bar y_A)=\left(1-\frac nN\right)\frac{S^2}{n}=\frac{N-n}{N-1}\frac{\sigma_N^2}{n}.
$$

Thus $1-n/N$ is the [variance](variance-split.md) factor relative to $S^2/n$, while $(N-n)/(N-1)$ is the exact [variance](variance-split.md) ratio to independent uniform [sampling with replacement](sampling-with-replacement.md), whose [sample mean](sample-mean.md) has [variance](variance-split.md) $\sigma_N^2/n$. The [standard error](standard-error.md) uses the square root of the corresponding factor. These formulas agree because $\sigma_N^2=(N-1)S^2/N$; the denominator convention must be specified. The [sample mean under simple random sampling](sample-mean-under-simple-random-sampling.md) gives a derivation and an exact six-value example.

## ↑ Ancestors (8)

1. [Hypergeometric distribution](hypergeometric-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Finite population correction](finite-population-correction.md)
- [Finite population variance](finite-population-variance.md)
- [Hypergeometric distribution](hypergeometric-distribution.md)
- [Multivariate hypergeometric distribution](multivariate-hypergeometric-distribution.md)
- [Sample mean under simple random sampling](sample-mean-under-simple-random-sampling.md)
- [Sampling fraction](sampling-fraction.md)
- [Sampling without replacement](sampling-without-replacement.md)

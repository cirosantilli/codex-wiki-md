# Jackknife bias correction

↑ **Parent:** [Statistical inference](statistical-inference-split.md)

The [jackknife bias correction](jackknife-bias-correction.md) uses [jackknife resampling](jackknife-resampling.md) to estimate and subtract the [bias of an estimator](bias-of-an-estimator.md). Here $T_n$ denotes the original [estimator](estimator.md), $T_{(-i)}$ its version after deleting observation $i$, and $\overline T_J=n^{-1}\sum_{i=1}^nT_{(-i)}$ the [mean](expected-value.md) of those versions. For [sample size](sample-size.md) $n>1$, define

$$
\widehat B_n=(n-1)(\overline T_J-T_n),\qquad
\widetilde T_J=T_n-\widehat B_n=nT_n-(n-1)\overline T_J.
$$

The sign matters: a negative estimated [bias](bias-of-an-estimator.md) increases the corrected value. The original [estimator](estimator.md) and all deletion versions must target the same [estimand](estimand.md) and use the same estimation rule at their respective [sample sizes](sample-size.md). The definition alone does not make $\widetilde T_J$ an [unbiased estimator](unbiased-estimator.md).

For an exact worked example, take the [empirical variance](empirical-variance.md)

$$
T_n=\frac1n\sum_{i=1}^n(X_i-\overline X_n)^2.
$$

On $(1,2,3,4,10)$, the [sample mean](sample-mean.md) is $4$ and $T_5=50/5=10$. Each deletion [empirical variance](empirical-variance.md) is recomputed around its own deletion [sample mean](sample-mean.md), with divisor $4$, giving

$$
(T_{(-1)},\ldots,T_{(-5)})
=(9.6875,11.25,12.1875,12.5,1.25),\qquad
\overline T_J=9.375.
$$

For instance, deleting $10$ leaves $(1,2,3,4)$, whose [sample mean](sample-mean.md) is $2.5$ and whose [empirical variance](empirical-variance.md) is $1.25$. The correction on the full [statistical sample](statistical-sample.md) is

$$
\widehat B_5=4(9.375-10)=-2.5,\qquad
\widetilde T_J=10-(-2.5)=12.5.
$$

The same data thus give a [jackknife variance estimator](jackknife-variance-estimator.md) of $2.5$ for the [sample mean](sample-mean.md), and a corrected [empirical variance](empirical-variance.md) of $12.5$; these are different [estimands](estimand.md).

<a id="image-two-uses-of-the-same-deletions-sampling-variance-and-jackknife-bias-correction"></a>
![](jackknife-variance-bias.png)

**[Figure 12](#image-two-uses-of-the-same-deletions-sampling-variance-and-jackknife-bias-correction). Two uses of the same deletions: sampling variance and jackknife bias correction**. The left panel plots contributions to the [jackknife variance estimator](jackknife-variance-estimator.md) of the [sample mean](sample-mean.md), summing to $2.5$. The right panel plots the five deletion [empirical variances](empirical-variance.md) and their [mean](expected-value.md) $9.375$, then compares the original [empirical variance](empirical-variance.md) $10$ with the corrected [sample variance](sample-variance.md) $12.5$.

The exact equality with the usual [sample variance](sample-variance.md) is not an accident of these numbers. For any data with $n>1$, write $Q=\sum_i(x_i-\overline x)^2=nT_n$. Removing $x_i$ changes this sum to $Q-n(x_i-\overline x)^2/(n-1)$, so

$$
T_{(-i)}=\frac{Q}{n-1}-\frac{n(x_i-\overline x)^2}{(n-1)^2},\qquad
\overline T_J=\frac{n(n-2)}{(n-1)^2}T_n,\qquad
\widetilde T_J=\frac{n}{n-1}T_n=s_n^2.
$$

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with finite second [moment](moment.md) and population [variance](variance-split.md) $\sigma^2$, the [expectation](expected-value.md) is $\mathbb E T_n=(1-1/n)\sigma^2$. Its [bias](bias-of-an-estimator.md) is exactly $-\sigma^2/n$; [jackknife bias correction](jackknife-bias-correction.md) removes it exactly in this example. Thus $s_n^2$ is an [unbiased estimator](unbiased-estimator.md) of $\sigma^2$ under these assumptions, including $n=2$ where each deletion [empirical variance](empirical-variance.md) is zero.

More generally, suppose the [bias](bias-of-an-estimator.md) has a regular expansion at both [sample sizes](sample-size.md) $n$ and $n-1$, with coefficients $a,b$ independent of $n$:

$$
B_n=\mathbb E T_n-\theta=\frac an+\frac b{n^2}+O(n^{-3}).
$$

Under [independent and identically distributed](independent-and-identically-distributed-random-variables.md) sampling, each deletion [estimator](estimator.md) has the same [expectation](expected-value.md) as $T_{n-1}$. Hence the corrected [bias](bias-of-an-estimator.md) is

$$
\mathbb E\widetilde T_J-\theta=nB_n-(n-1)B_{n-1}=O(n^{-2}),
\qquad n\frac an-(n-1)\frac a{n-1}=0.
$$

The leading $O(n^{-1})$ term cancels; the remaining [bias](bias-of-an-estimator.md) need not vanish. The $O$ notation is [big O notation](big-o-notation.md). This argument presumes the expansion, rather than proving it for every [statistic](statistic.md); the regularity conditions discussed for the [jackknife variance estimator](jackknife-variance-estimator.md) and [statistical dependence](statistical-dependence.md) still require care. Shalizi's [jackknife notes, Section 5.1](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) develop the cancellation argument and cite Quenouille's [Notes on Bias in Estimation, Biometrika 43(3–4), 353–360 (1956)](https://academic.oup.com/biomet/article-abstract/43/3-4/353/345190).

**Table of contents**

- [Sample variance](sample-variance.md)
  - [Empirical variance](empirical-variance.md)
  - [Pooled sample variance](pooled-sample-variance.md)

## ↑ Ancestors (5)

1. [Statistical inference](statistical-inference-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Empirical variance](empirical-variance.md)
- [Jackknife bias correction](jackknife-bias-correction.md)
- [Jackknife resampling](jackknife-resampling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/28j/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/28k/a/solution.md)

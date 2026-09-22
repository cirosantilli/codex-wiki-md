<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [weakly stationary process](../../../../../../weakly-stationary-process.md), every observation has the same finite [expectation](../../../../../../expected-value.md) $\mu$. Linearity of [expectation](../../../../../../expected-value.md), without any assumption of [independence](../../../../../../independent-random-variables.md), gives

$$
\boxed{\mathbb E\overline Y=\frac1n\sum_i\mathbb E Y_i=\mu.}
$$

The [variance](../../../../../../variance-split.md) is a sum of all pairwise [covariances](../../../../../../covariance.md):

$$
\operatorname{Var}(\overline Y)=\frac1{n^2}\sum_{i,j=1}^n\gamma(i-j).
$$

For a real-valued [weakly stationary process](../../../../../../weakly-stationary-process.md), the [autocovariance](../../../../../../autocovariance.md) is even. There are $n$ pairs at lag zero and $n-h$ pairs in each direction at positive lag $h$. Therefore

$$
\boxed{\operatorname{Var}(\overline Y)=\frac{\gamma(0)}n+\frac2{n^2}\sum_{h=1}^{n-1}(n-h)\gamma(h).}
$$

Positive [autocovariances](../../../../../../autocovariance.md) inflate the uncertainty relative to the independent-observation formula; negative terms may reduce it. An [unbiased estimator](../../../../../../unbiased-estimator.md) need not have [variance](../../../../../../variance-split.md) tending to zero: a process consisting of the same random variable at every time is weakly stationary, but averaging cannot reduce its [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

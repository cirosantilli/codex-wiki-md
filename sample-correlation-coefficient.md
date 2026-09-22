# Sample correlation coefficient

↑ **Parent:** [Covariance](covariance.md)

For paired observations $(x_i,y_i)$, the [sample correlation coefficient](sample-correlation-coefficient.md) is

$$
r_{XY}=\frac{\sum_i(x_i-\overline x)(y_i-\overline y)}
{\sqrt{\sum_i(x_i-\overline x)^2\sum_i(y_i-\overline y)^2}}.
$$

It is the normalized [inner product](inner-product-split.md) of the centered data [vectors](vector.md), or the [sample covariance](sample-covariance.md) divided by the product of the corresponding sample [standard deviations](standard-deviation.md). The choice of divisor $n$ or $n-1$ cancels when used consistently in all three quantities. It is undefined if either centered data [vector](vector.md) is zero, which occurs when that variable is constant in the observed [statistical sample](statistical-sample.md).

For $x=(1,2,3,4)$ and $y=(2,1,4,3)$, both [sample means](sample-mean.md) are $2.5$. The sum of centered products is $3$, and each sum of centered squares is $5$, hence **the sample correlation coefficient is $3/5=0.6$**. This is a summary of these four observed pairs; it is not automatically the population [Pearson correlation coefficient](pearson-correlation-coefficient.md). [Philip Stark, Computing the correlation coefficient](https://www.stat.berkeley.edu/~stark/SticiGui/Text/computeR.htm) explains the centered and standardized calculation.

**Table of contents**

- [Sample correlation matrix](sample-correlation-matrix.md)

## ↑ Ancestors (8)

1. [Covariance](covariance.md)
2. [Variance](variance-split.md)
3. [Expected value](expected-value-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/4/b/i/solution.md)
- [Sample correlation coefficient](sample-correlation-coefficient.md)
- [Sample correlation matrix](sample-correlation-matrix.md)

<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first matrix contains the leave-one-out samples, and each element of `vect` is their [sample mean](../../../../../../sample-mean.md). For $n\geq2$,

$$
\overline x_{(-i)}=\frac{n\overline x-x_i}{n-1},\qquad
\frac1n\sum_i\overline x_{(-i)}=\overline x.
$$

Thus R4a computes the [Jackknife variance estimator](../../../../../../jackknife-variance-estimator.md) of the full [sample mean](../../../../../../sample-mean.md):

$$
\frac{n-1}{n}\sum_i(\overline x_{(-i)}-\overline x)^2
=\frac1{n(n-1)}\sum_i(x_i-\overline x)^2=\boxed{s_x^2/n},
$$

where $s_x^2$ is the unbiased [sample variance](../../../../../../sample-variance.md). R5a computes the estimated bias used in [jackknife bias correction](../../../../../../jackknife-bias-correction.md). The identity for the average leave-one-out [sample mean](../../../../../../sample-mean.md) gives **R5a = 0**, apart from floating-point rounding.

**The second printed loop contains an indexing error: its row index is `i`, although its loop variable is `b`.** Literally, after the first block, `i` equals $n$. When $n\leq199$, every iteration overwrites row $n$ of the new matrix; the other rows remain missing. Hence `vect` contains one finite mean and 198 missing entries. R's default sorting removes missing entries, leaving a vector of length one, so selecting its fifth and 195th entries gives **R7b = `c(NA, NA)`**. If $n>199$, the matrix assignment is out of bounds; if the second block runs independently with `i` undefined, it fails even earlier. This is a source error, not a property of the [bootstrap](../../../../../../bootstrapping-statistics.md).

Replacing just the row index by `b` gives the intended algorithm: draw 199 independent [bootstrap samples](../../../../../../bootstrap-sample.md) and sort their [sample means](../../../../../../sample-mean.md) as $s_1\leq\cdots\leq s_{199}$. The two indices are $200(0.05/2)=5$ and $200(1-0.05/2)=195$, so

$$
\boxed{\text{intended R7b}=(s_5,s_{195}).}
$$

These are the endpoints of an approximate 95% [percentile bootstrap confidence interval](../../../../../../percentile-bootstrap-confidence-interval.md) for the population [mean](../../../../../../expected-value.md). Their actual numerical values depend on the supplied data and random draws, which are not specified. They are not the reflected endpoints of a [basic bootstrap confidence interval](../../../../../../basic-bootstrap-confidence-interval.md), and the choice of ranks does not guarantee exact finite-sample coverage.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

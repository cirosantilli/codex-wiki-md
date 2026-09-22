<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Standard one-dimensional [Brownian motion](../../../../../brownian-motion-split.md) is a real process with $B_0=0$, continuous paths almost surely, and increments $B_t-B_s\sim N(0,t-s)$ [independent](../../../../../independent-random-variables.md) of the past at time $s$, for $0\le s<t$. These conditions determine its entire [finite-dimensional distribution](../../../../../finite-dimensional-distribution.md) family.

The [Wiener theorem](../../../../../wiener-theorem.md) asserts that such a process exists, equivalently that there is a unique [Wiener measure](../../../../../wiener-measure.md) on $C_0([0,\infty),\mathbb R)$ under which the coordinate process has these properties. To construct it, prescribe centered multivariate [normal](../../../../../normal-distribution.md) laws with [covariance](../../../../../covariance.md) $\mathbb E B_sB_t=\min(s,t)$. This [covariance](../../../../../covariance.md) is [positive semidefinite](../../../../../positive-semidefinite-matrix.md) because

$$
\sum_{i,j}c_ic_j\min(t_i,t_j)=\int_0^\infty\left(\sum_i c_i\mathbf1_{[0,t_i]}(u)\right)^2du\ge0.
$$

The laws are consistent under removing coordinates, so the [Kolmogorov extension theorem](../../../../../kolmogorov-extension-theorem.md) constructs the process. [Normal](../../../../../normal-distribution.md) increments have [fourth moment](../../../../../fourth-moment.md) $\mathbb E|B_t-B_s|^4=3|t-s|^2$. The [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md) therefore supplies a continuous modification, retaining all the prescribed finite-dimensional laws and hence the [independent](../../../../../independent-random-variables.md) [normal](../../../../../normal-distribution.md) increments. Apply this on every compact time interval, taking consistent versions; continuity and equality at rational times make them agree on overlaps. The resulting law on continuous-path space is unique because evaluations at rational times generate its [Borel sigma-algebra](../../../../../borel-sigma-algebra.md). This is a proof sketch of the existence theorem, [independent](../../../../../independent-random-variables.md) of the random-walk limit in Question 5.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

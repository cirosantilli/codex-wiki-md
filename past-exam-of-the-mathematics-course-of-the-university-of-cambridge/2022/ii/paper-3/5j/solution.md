<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

The log density is

$$
-\log(2\sigma)-\frac{|y-\mu|}{\sigma}.
$$

Its kink occurs at the unknown location $\mu$, so its parameter dependence cannot be separated into a fixed finite-dimensional statistic of $y$ and the smooth canonical form required of an exponential dispersion family. Thus the two-parameter location-scale [Laplace distribution](../../../../../laplace-distribution.md) is not such a family.

For independent observations, the [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\beta,\sigma)
=-n\log(2\sigma)-\frac1\sigma
\sum_{i=1}^n|Y_i-X_i^T\beta|
=-n\log(2\sigma)-\frac{S(\beta)}{\sigma}.
$$

For every fixed $\sigma>0$, maximizing this expression in $\beta$ is equivalent to minimizing $S(\beta)$. Hence

$$
\boxed{
\widehat\beta\in\operatorname*{arg\,min}_\beta
\sum_{i=1}^n|Y_i-X_i^T\beta|
},
$$

the [least absolute deviations](../../../../../laplace-regression.md) estimator. At this value,

$$
\frac{\partial\ell}{\partial\sigma}
=-\frac n\sigma+\frac{S(\widehat\beta)}{\sigma^2},
$$

so, in the nondegenerate case $S(\widehat\beta)>0$,

$$
\boxed{\widehat\sigma=\frac{S(\widehat\beta)}n}.
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="9/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For this rate parametrization of the [Laplace distribution](../../../../../../../laplace-distribution.md), $\mu$ is its [mean](../../../../../../../expected-value-split.md) and [median](../../../../../../../median.md). By [symmetry](../../../../../../../symmetry-physics.md), $\mathbb E(X-\mu)=0$, while $|X-\mu|$ has [exponential distribution](../../../../../../../exponential-distribution.md) with rate $\lambda$, so

$$
\operatorname{Var}(X)=\mathbb E|X-\mu|^2
=\int_0^\infty r^2\lambda e^{-\lambda r}\,dr=\frac2{\lambda^2}.
$$

The [integral](../../../../../../../integral-split.md) follows by two applications of [integration by parts](../../../../../../../integration-by-parts.md). The [central limit theorem](../../../../../../../central-limit-theorem.md) therefore gives

$$
\frac{\sqrt n(\overline X-\mu)}{\sqrt2/\lambda}
\ \xrightarrow{d}\ N(0,1).
$$

With known $\lambda$ and the supplied cutoff 2, an approximate 95% [confidence interval](../../../../../../../confidence-interval.md) is

$$
\boxed{\left[\overline x-\frac{2\sqrt2}{\lambda\sqrt n},\ 
\overline x+\frac{2\sqrt2}{\lambda\sqrt n}\right].}
$$

This [known-rate Laplace location confidence interval](../../../../../../../known-rate-laplace-location-confidence-interval.md) uses the [sample mean](../../../../../../../sample-mean.md); the later [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) of location need not be used to construct this valid asymptotic [confidence interval](../../../../../../../confidence-interval.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

<h1 id="o/o5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A=(X^TX)^{-1}X^T$. Since $AX=I_p$,

$$
\widehat\theta=\theta+A\epsilon.
$$

The errors have mean zero and [covariance matrix](../../../../../covariance-matrix.md) $\sigma^2I_n$. Therefore

$$
\boxed{\mathbb E\widehat\theta=\theta,\qquad
\operatorname{Cov}(\widehat\theta)=\sigma^2AA^T
=\sigma^2(X^TX)^{-1}.}
$$

Thus $\widehat\theta$ is an [unbiased estimator](../../../../../unbiased-estimator.md). In addition, the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) is preserved by [linear maps](../../../../../linear-map.md), so $\widehat\theta$ is [multivariate normal](../../../../../multivariate-normal-distribution.md) with the displayed mean and [covariance matrix](../../../../../covariance-matrix.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

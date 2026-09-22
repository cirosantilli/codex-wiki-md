<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

[Wilks theorem](../../../../../wilks-theorem.md) states that, under an interior null parameter and the usual identifiability, smoothness and nonsingular-information regularity conditions, $-2\log\Lambda$ for nested models converges under the null to a chi-square distribution with degrees of freedom equal to the difference of parameter [dimensions](../../../../../dimension-vector-space.md). Boundary or nonidentifiable nulls need not have this distribution.

Write $\bar X=n^{-1}\sum X_i$, $Q=\sum(X_i-\bar X)^2$ and $S=\sum X_i^2=Q+n\bar X^2$. The unrestricted maximum-likelihood estimates are $\widehat\mu=\bar X$ and $\widehat\sigma^2=Q/n$. Under the null the [variance](../../../../../variance-split.md) estimate is $S/n$. Substituting both maxima into the Gaussian likelihood gives

$$
\boxed{\Lambda=(Q/S)^{n/2},\qquad -2\log\Lambda=n\log\left(1+\frac{n\bar X^2}{Q}\right)\ \overset{H_0}{\approx}\ \chi_1^2.}
$$

This is for $n\ge2$, with positive true [variance](../../../../../variance-split.md); $Q>0$ almost surely. The lost parameter [dimension](../../../../../dimension-vector-space.md) is one, even though [variance](../../../../../variance-split.md) is estimated in both models.

The two-sided [Student t-test](../../../../../student-s-t-test.md) uses $T=\sqrt n\bar X/s$, where $s^2=Q/(n-1)$, and rejects when $|T|>t_{n-1,1-\alpha/2}$. Under the null $T$ has exactly the [Student t-distribution](../../../../../student-s-t-distribution.md) with $n-1$ degrees of freedom. The likelihood-ratio statistic is

$$
-2\log\Lambda=n\log(1+T^2/(n-1))=T^2+o_P(1)
$$

under the null, so its chi-square approximation agrees asymptotically with the squared asymptotic standard-normal t statistic. In fact the expression is strictly increasing in $T^2$: with exact finite-sample calibration the tests have **identical rejection regions for every $n$**, not just approximately for large samples.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

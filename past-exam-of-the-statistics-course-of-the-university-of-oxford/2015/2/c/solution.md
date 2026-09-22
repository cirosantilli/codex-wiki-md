<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $a=x_{(1)}=\min_i x_i$, $T=\sum_i x_i$ and $\overline x=T/n$. For nondegenerate data from the shifted [exponential distribution](../../../../exponential-distribution.md), the [likelihood function](../../../../likelihood-function.md) is

$$
L(\theta,\beta)=\beta^{-n}
\exp\!\left[-\frac{T-n\theta}{\beta}\right]
\mathbf1_{\{0\leq\theta\leq a\}}.
$$

For fixed feasible $\theta$, differentiating its [log-likelihood](../../../../log-likelihood.md) with respect to $\beta$ gives

$$
-\frac n\beta+\frac{T-n\theta}{\beta^2}=0,
\qquad \widehat\beta(\theta)=\overline x-\theta.
$$

The derivative changes from positive to negative there. Substituting gives the profile [likelihood](../../../../likelihood-function.md) $e^{-n}(\overline x-\theta)^{-n}$, which increases with $\theta$. Therefore the unrestricted [maximum-likelihood estimates](../../../../maximum-likelihood-estimator.md) are

$$
\widehat\theta=a,\qquad \widehat\beta=\overline x-a,
$$

while under the [null hypothesis](../../../../null-hypothesis.md) $\theta=0$ the estimate is $\widetilde\beta=\overline x$. Their [likelihood ratio](../../../../likelihood-ratio.md) is

$$
R=\frac{\overline x^{-n}e^{-n}}{(\overline x-a)^{-n}e^{-n}}
=\left(1-\frac a{\overline x}\right)^n.
$$

Since the [likelihood-ratio test](../../../../likelihood-ratio-test.md) rejects for small $R$, the requested form is obtained with

$$
\boxed{g(x_1,\ldots,x_n)=\frac{x_{(1)}}{\overline x}
=\frac{n\min_i x_i}{\sum_i x_i},\qquad
C=\{x:(1-g(x))^n\leq k\}.}
$$

The formulas assume $\overline x>a$, which holds almost surely for a continuous sample with $n\geq2$; coincident observations give an unbounded unrestricted [likelihood](../../../../likelihood-function.md) and can be treated by its supremum.

An exact calibration is available and also explains why [Wilks theorem](../../../../wilks-theorem.md) should not be applied here. Under the null, the [memoryless property](../../../../memorylessness-of-the-exponential-distribution.md) makes $A=nX_{(1)}$ and $D=\sum_i(X_i-X_{(1)})$ independent [gamma distributions](../../../../gamma-distribution.md) with common scale $\beta$ and shapes $1$ and $n-1$. By [beta sampling by gamma ratios](../../../../beta-sampling-by-gamma-ratios.md),

$$
1-g=\frac{D}{A+D}\sim\operatorname{Beta}(n-1,1).
$$

Consequently, for $0\leq k\leq1$,

$$
\Pr_0(R\leq k)=k^{(n-1)/n},\qquad
\boxed{k_\alpha=\alpha^{n/(n-1)}.}
$$

This yields an exact [test size](../../../../size-of-a-statistical-test.md) $\alpha$, independent of the unknown scale. The support endpoint and boundary null make this a [likelihood-ratio test for an exponential support endpoint](../../../../likelihood-ratio-test-for-an-exponential-support-endpoint.md), with a different calibration from a regular one-parameter test.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="o/5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a sample of size $n\ge2$, define

$$
\overline X=\frac1n\sum_{i=1}^nX_i,\qquad
S^2=\frac1{n-1}\sum_{i=1}^n(X_i-\overline X)^2.
$$

For the zero-mean Gaussian sample, the standardized [vector](../../../../../vector.md) $(X_1/\sigma,\ldots,X_n/\sigma)$ has independent [standard normal](../../../../../standard-normal-distribution.md) coordinates. Apply an [orthogonal transformation](../../../../../orthogonal-transformation.md) whose first row is $(1,\ldots,1)/\sqrt n$. The resulting coordinates $Z_1,\ldots,Z_n$ remain independent [standard normals](../../../../../standard-normal-distribution.md): their [joint density](../../../../../joint-probability-density.md) depends only on squared Euclidean length and the transformation has unit absolute Jacobian. Its first coordinate is $Z_1=\sqrt n\,\overline X/\sigma$, while [orthogonal decomposition](../../../../../orthogonal-decomposition-by-a-closed-subspace.md) gives

$$
\sum_{j=2}^nZ_j^2=\frac1{\sigma^2}\sum_i(X_i-\overline X)^2
=\frac{(n-1)S^2}{\sigma^2}.
$$

Thus

$$
\boxed{\frac{\sqrt n}{\sigma}\overline X\sim N(0,1),\quad
\frac{n-1}{\sigma^2}S^2\sim\chi^2_{n-1},\quad\overline X\text{ and }S^2\text{ independent}.}
$$

The ratio of the first independent [standard normal](../../../../../standard-normal-distribution.md) and the [square root](../../../../../square-root.md) of the normalized chi-square variable has a Student [probability distribution](../../../../../probability-distribution-split.md), giving

$$
\boxed{\frac{\sqrt n\,\overline X}{S}\sim t_{n-1}.}
$$

For the paired height observations, form one cross-minus-self difference per pot. The sampling units for this test are the fifteen differences, not thirty separate plant heights. Under the usual independent normal model for differences, a null mean of zero gives a $t_{14}$ statistic. The observed statistic is

$$
t_{\rm obs}=\frac{2.607}{4.713/\sqrt{15}}.
$$

For the two-sided alternative, reject at [significance level](../../../../../significance-level.md) $\delta$ if $|t_{\rm obs}|>t_{14,1-\delta/2}$. Its two-sided $p$-value is $2[1-F_{t_{14}}(|t_{\rm obs}|)]$. This uses the recorded values without performing the numerical calculation forbidden by the question. The normal difference model is what makes the small-sample Student calibration exact.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [5](../../5.md)
3. [O](../../../o.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The standardized observations $X_i/\sigma$ are independent standard [normal random variables](../../../../gaussian-random-variable.md). By the definition of the [chi-squared distribution](../../../../chi-squared-distribution.md),

$$
Q=\frac{\sum_iX_i^2}{\sigma^2}\sim\chi_n^2.
$$

Its distribution is continuous, so $F_n(c_2)-F_n(c_1)=1-\alpha$ gives the required [probability](../../../../probability.md). Put $S=\sum_iX_i^2$. Solving $c_1<S/\sigma^2<c_2$ for the positive [variance](../../../../variance-split.md) reverses the reciprocal order. The exact [confidence interval](../../../../confidence-interval.md) is

$$
\boxed{\left(\frac S{F_n^{-1}(1-\alpha/2)},\frac S{F_n^{-1}(\alpha/2)}\right).}
$$

The mean is known to be zero, so the degrees of freedom are $n$, not $n-1$. Coverage is exactly $1-\alpha$ under the stated normal model.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For fixed $n$, the [likelihood ratio](../../../../../likelihood-ratio.md) is strictly decreasing as $t^2$ increases. A [likelihood-ratio test](../../../../../likelihood-ratio-test.md) rejects for small $\lambda$, so its rejection rule is equivalently large $|t|$. Under the [null hypothesis](../../../../../null-hypothesis.md), the standard [normal distribution](../../../../../normal-distribution.md) and [chi-squared distribution](../../../../../chi-squared-distribution.md) results give independent quantities

$$
\frac{\sqrt n(\overline Y-\mu_0)}{\sigma}\sim N(0,1),\qquad
\frac{(n-1)s_Y^2}{\sigma^2}\sim\chi^2_{n-1}.
$$

Their ratio therefore has [Student's t-distribution](../../../../../student-s-t-distribution.md) with $n-1$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The exact level-$\alpha$ rule is

$$
\boxed{|t|>t_{n-1,\,1-\alpha/2}.}
$$

This is precisely the two-sided [Student's t-test](../../../../../student-s-t-test.md); choosing the corresponding cutoff for $\lambda$ yields the same rejection region and the same [p-value](../../../../../p-value.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

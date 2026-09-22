<h1 id="o/o4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The log [likelihood ratio](../../../../../likelihood-ratio.md) statistic comparing the unrestricted fit with the [independence](../../../../../independent-random-variables.md) fit is

$$
\begin{aligned}
\Lambda&=2\{\ell(\widehat\theta)-\ell(\widehat\theta^{\,0})\}\\
&=2\sum_{i,j}n_{ij}\log\left(\frac{n_{ij}/N}{n_{i.}n_{.j}/N^2}\right)
=\boxed{2\sum_{i,j}n_{ij}\log\left(\frac{n_{ij}N}{n_{i.}n_{.j}}\right)}.
\end{aligned}
$$

The unrestricted model has $rc-1=8$ free parameters. [Independence](../../../../../independent-random-variables.md) has $(r-1)+(c-1)=4$, so the difference is $(r-1)(c-1)=4$. By [Wilks theorem](../../../../../wilks-theorem.md), under the [null hypothesis](../../../../../null-hypothesis.md) the statistic has asymptotically a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $4$ degrees of freedom, rather than $6$, $8$, or $9$.

For the supplied statistic, the approximate [p-value](../../../../../p-value.md) is $1-F_4(11.8)=0.02$. Thus **reject [independence](../../../../../independent-random-variables.md) at the 5% level**, but not at the 1% level: the data provide evidence of an association. The approximation is reasonable here; the smallest fitted cell count is $27\cdot99/299\approx8.94$, so all fitted counts exceed $5$. The [statistical hypothesis test](../../../../../statistical-hypothesis-test-split.md) concerns association, not a causal effect of personality.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [O4](../../o4.md)
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

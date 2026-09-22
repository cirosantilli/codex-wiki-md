<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Let $p_{\rm old}$ and $p_{\rm new}$ be the underlying full-recovery probabilities. The two-sided [statistical hypothesis test](../../../../../statistical-hypothesis-test.md) is

$$
H_0:p_{\rm old}=p_{\rm new},\qquad
H_1:p_{\rm old}\ne p_{\rm new}.
$$

Use the [Pearson chi-squared test of homogeneity](../../../../../pearson-chi-squared-test-of-homogeneity.md) for the two independent groups. Under $H_0$, the pooled recovery estimate is $\widehat p=56/100=0.56$, so each row has expected counts 28 recovered and 22 not recovered. All expected counts comfortably exceed five. The [Pearson chi-squared statistic for contingency tables](../../../../../pearson-chi-squared-statistic-for-contingency-tables.md) is

$$
X^2=2\left(\frac{3^2}{28}+\frac{3^2}{22}\right)
=\frac{225}{154}\approx1.461.
$$

The asymptotic reference distribution is a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $(2-1)(2-1)=1$ degree of freedom. Since $1.461<3.84$, **do not reject equal recovery probabilities at the 5% level**. The observed recovery proportions, 0.50 and 0.62, do not provide statistically significant evidence of a difference in this trial. This conclusion does not prove that the procedures have identical recovery probabilities.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

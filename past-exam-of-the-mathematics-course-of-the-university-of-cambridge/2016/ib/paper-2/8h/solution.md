<h1 id="8h/solution">Solution</h1>

↑ **Parent:** [8H](../8h.md)

Under the null hypothesis the three outcome probabilities are the same in the two independent samples. The pooled row totals are $50,20,30$, and both column totals are $50$, out of a total of $100$. Thus the expected counts in each column are $25,10,15$. These exceed the usual small-count threshold for the asymptotic [Pearson chi-squared test of homogeneity](../../../../../pearson-chi-squared-test-of-homogeneity.md).

The [Pearson chi-squared statistic for contingency tables](../../../../../pearson-chi-squared-statistic-for-contingency-tables.md) is

$$
X^2=2\left(\frac{(28-25)^2}{25}+\frac{(4-10)^2}{10}+\frac{(18-15)^2}{15}\right)=\boxed{9.12}.
$$

Under the null, its asymptotic [chi-squared distribution](../../../../../chi-squared-distribution.md) has $(3-1)(2-1)=2$ [degrees of freedom](../../../../../degree-of-freedom.md). Equivalently, the two independent three-category samples have four probability parameters unrestricted and two under the common-probability null. The $1\%$ upper-tail critical value is $9.21$.

Since $9.12<9.21$, **do not reject the equal-effect hypothesis at the 1% level**. For two [degrees of freedom](../../../../../degree-of-freedom.md), the approximate [p-value](../../../../../p-value.md) is $e^{-9.12/2}\simeq0.01046$, just above $0.01$. This is a decision at the specified [significance level](../../../../../significance-level.md), not evidence that the two outcome distributions have been proved identical.

## ↑ Ancestors (10)

1. [8H](../8h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

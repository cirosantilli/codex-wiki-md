<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Under the [null hypothesis](../../../../../null-hypothesis.md) that treatment and recovery are independent, estimate each expected cell count by

$$
E_{ij}=\frac{(\text{row total})(\text{column total})}{N}
$$

and form the [Pearson chi-squared test of independence](../../../../../pearson-chi-squared-test-of-independence.md) statistic $\chi^2=\sum(O-E)^2/E$. For a $2\times2$ table its asymptotic null law is a [chi-squared distribution](../../../../../chi-squared-distribution.md) with one [degree of freedom](../../../../../degree-of-freedom.md). A second-order [Taylor expansion](../../../../../taylor-expansion.md) of the [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) statistic $-2\log\Lambda$ around the fitted counts gives this Pearson statistic, which explains its asymptotic null distribution.

Writing the four residuals over their fitted counts and simplifying gives

$$
\boxed{\chi^2=\frac{(ad-bc)^2(a+b+c+d)}{(a+b)(c+d)(a+c)(b+d)}.}
$$

For $(a,b,c,d)=(50,10,15,5)$,

$$
\chi^2=\frac{80}{117}\approx0.684,
$$

whose one-degree-of-freedom [p-value](../../../../../p-value.md) is about $0.41$. There is no evidence of an effect. One fitted count is only $3.75$, however, so the chi-squared approximation is questionable; [Fisher's exact test](../../../../../fisher-s-exact-test.md) would be preferable.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

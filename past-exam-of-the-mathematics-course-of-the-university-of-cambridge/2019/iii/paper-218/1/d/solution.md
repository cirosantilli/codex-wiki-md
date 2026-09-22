<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For observed proportions $y_i$ and fitted proportions $\widehat p_i$, the [binomial deviance](../../../../../../binomial-deviance.md) is

$$
D=2\sum_i m_i\left[
y_i\log\frac{y_i}{\widehat p_i}
+(1-y_i)\log\frac{1-y_i}{1-\widehat p_i}
\right].
$$

A second-order Taylor expansion around $y_i=\widehat p_i$ gives

$$
D\approx\sum_i\frac{m_i(y_i-\widehat p_i)^2}
{\widehat p_i(1-\widehat p_i)},
$$

the generalized [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md). Under the fitted binomial model this is approximately $\chi^2_{4-3}=\chi^2_1$. The observed deviance is $1.6102$, whose upper-tail probability is about $0.20$. Since this exceeds $0.05$, **there is no significant evidence of overdispersion**.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

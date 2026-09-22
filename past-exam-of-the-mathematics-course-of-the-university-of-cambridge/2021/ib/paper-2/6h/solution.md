<h1 id="6h/solution">Solution</h1>

↑ **Parent:** [6H](../6h.md)

Under the null hypothesis of independence between treatment and outcome, the expected counts in each treatment row are one half of the column totals:

$$
(10,20,10,10).
$$

The [Pearson chi-squared test of independence](../../../../../pearson-chi-squared-test-of-independence.md) statistic is

$$
\begin{aligned}
X^2
&=2\left(
\frac{(14-10)^2}{10}
+\frac{(21-20)^2}{20}
+\frac{(10-10)^2}{10}
+\frac{(5-10)^2}{10}
\right)\\
&=\boxed{8.30}.
\end{aligned}
$$

The number of [degrees of freedom](../../../../../degree-of-freedom.md) is

$$
(2-1)(4-1)=3.
$$

At the 5% level the critical value is $7.81$. Since $8.30>7.81$, we reject the null hypothesis and find statistically significant evidence that the drug and placebo have different effects.

## ↑ Ancestors (10)

1. [6H](../6h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Use the [Pearson chi-squared goodness-of-fit test](../../../../../pearson-chi-squared-goodness-of-fit-test.md). Under the [null hypothesis](../../../../../null-hypothesis.md), each count has the specified [binomial distribution](../../../../../binomial-distribution.md), and no parameter is estimated from the data. The seven mutually exclusive classes give $7-1=6$ [degrees of freedom](../../../../../degree-of-freedom.md). Their expected counts are all at least five, so the usual [chi-squared asymptotic approximation](../../../../../chi-squared-asymptotic-approximation.md) does not require pooling. The computed statistic is

$$
X^2=\frac{(-2)^2}{5}+\frac{(-9)^2}{30}+\frac{10^2}{75}+\frac{10^2}{100}
+\frac{(-13)^2}{75}+\frac{2^2}{30}+\frac{2^2}{5}
=\boxed{9.02}.
$$

Since $9.02<12.59$, **do not reject fairness at the 5% level**. The approximate $p$-value is $0.172$. This conclusion concerns agreement with the specified independent fair-coin count model; a nonrejection is not proof of fairness.

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

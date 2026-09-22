<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [mean](../../../../../../expected-value.md) ratio is $R=(\lambda e^\beta)/\lambda=e^\beta$, so its logarithm is exactly $\beta$; the baseline coefficient $\alpha$ cancels. Under the stated asymptotic [normal approximation](../../../../../../normal-approximation.md), the [Wald confidence interval](../../../../../../wald-confidence-interval.md) for $\beta$ is $0.69\pm1.96(0.15)=(0.396,0.984)$. Exponentiation is monotone and therefore preserves the interval's coverage event. Hence

$$
\boxed{\widehat R=e^{0.69}\simeq1.99,\qquad
R\text{ has approximate }95\%\text{ CI }(1.49,2.68).}
$$

The [standard error](../../../../../../standard-error.md) of $\alpha$ is not needed for this [confidence interval](../../../../../../confidence-interval.md): the [Poisson regression](../../../../../../poisson-regression.md) already supplies the [standard error](../../../../../../standard-error.md) of the contrast $\beta$. It would be incorrect to combine the two reported [standard errors](../../../../../../standard-error.md) as if the [mean](../../../../../../expected-value.md) ratio depended on both coefficients independently.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

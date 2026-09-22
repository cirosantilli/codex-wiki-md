<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

Under the [null hypothesis](../../../../../null-hypothesis.md) of equal population probabilities, the three counts have a [multinomial distribution](../../../../../multinomial-distribution.md) with probabilities $1/3$ and expected counts $100$ each. The [Pearson chi-squared goodness-of-fit test](../../../../../pearson-chi-squared-goodness-of-fit-test.md) uses

$$
X^2=\sum_{j=1}^3\frac{(O_j-100)^2}{100}
=\frac{(-8)^2+(-11)^2+19^2}{100}
=\boxed{5.46}.
$$

No probabilities have been estimated from the data, and the three counts sum to a fixed total. Hence the null reference [chi-squared distribution](../../../../../chi-squared-distribution.md) has $3-1=2$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The supplied $5\%$ upper critical value is $5.99$, and $5.46<5.99$. **At the 5% significance level there is insufficient evidence to reject equal popularity.**

The asymptotic [P-value](../../../../../p-value.md) is $\Pr(\chi_2^2\ge5.46)=e^{-5.46/2}\approx0.0652$. The expected counts are all large, so the approximation is appropriate if the sampled choices are independent and representative of this branch. The conclusion depends on the chosen [significance level](../../../../../significance-level.md); for instance, a $10\%$ test would reject. Nonrejection does not establish the [null hypothesis](../../../../../null-hypothesis.md), and a survey at one branch does not by itself justify a population claim about every branch.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Overdispersion](../../../../../../overdispersion.md) means that conditional variance exceeds the Poisson mean. Under a correctly specified Poisson model, the Pearson statistic is approximately chi-squared with $149$ residual degrees of freedom. Here

$$
X^2=149(1.3119)\simeq195.5,\qquad
\frac{X^2-149}{\sqrt{2(149)}}\simeq2.69>1.645,
$$

so a one-sided five-percent test rejects. The displayed model-based confidence interval is too narrow. A quasi-Poisson fit can multiply standard errors by $\sqrt{1.3119}$; [negative binomial regression](../../../../../../negative-binomial-regression.md) or a random-effects count model can model the extra variation directly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

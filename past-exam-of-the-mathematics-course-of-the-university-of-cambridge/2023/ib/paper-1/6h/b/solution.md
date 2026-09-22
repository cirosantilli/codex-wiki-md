<h1 id="6h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The null hypothesis is that mortality is independent of carbolic-acid use, equivalently that the two mortality probabilities are equal. The two-sided alternative is that they differ.

Use the [Chi-squared test of independence](../../../../../../chi-squared-test-of-independence.md), equivalently the likelihood-ratio statistic, with Pearson's statistic

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}},
$$

where $E_{ij}$ are the fitted counts under independence using the observed row and column totals. Under the null, $X^2$ is asymptotically $\chi^2_1$. A size-$\alpha$ test rejects when

$$
\boxed{X^2>\chi^2_{1,1-\alpha}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6H](../../6h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

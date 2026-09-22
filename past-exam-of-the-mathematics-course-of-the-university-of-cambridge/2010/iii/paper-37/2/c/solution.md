<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The reduced model combines the 0-, 3-, and 6-point categories. Relative to the full model, the null hypothesis is $\eta_3=\eta_6=0$, leaving the 9-point contrast unrestricted. These are two linear restrictions on an otherwise unchanged [normal linear model](../../../../../../normal-linear-model.md).

For nested normal models, the reduction in [residual sum of squares](../../../../../../residual-sum-of-squares.md) divided by $\sigma^2$ has a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with degrees of freedom equal to the number of restrictions. It is independent of the full model's residual variance estimate. Hence the [F-test](../../../../../../f-test.md) statistic is

$$
F=\frac{(22323-19512)/2}{19512/24}=1.728782\sim F_{2,24}\quad\text{under }H_0.
$$

It is below the supplied 5% critical value $3.402826$, so **do not reject equal effects for 0, 3, and 6 points**. There is insufficient evidence that separating those categories improves this additive model; this does not prove that their true premiums are identical.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

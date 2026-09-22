<h1 id="5j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The comparison is a [nested-model F-test](../../../../../../nested-model-f-test.md) of the three time-by-diet interaction coefficients, with null hypothesis that all are zero. The reduced [linear regression](../../../../../../linear-regression-split.md) model has a common time slope and four diet-specific intercepts; the full model permits four slopes. It has eight fitted coefficients and $579-8=571$ residual degrees of freedom.

$$
F=\frac{(34.381-31.589)/3}{31.589/571}\approx16.823,
\qquad \boxed{F\sim F_{3,571}\text{ under the null}}.
$$

The rounded sums of squares give the displayed approximation; the software reports $F=16.824$ using unrounded values. The quoted [p-value](../../../../../../p-value.md) $1.744\times10^{-10}$ gives overwhelming evidence against equal log-weight growth slopes across diets under the [normal linear model](../../../../../../normal-linear-model.md) assumptions. Thus **reject the common-slope hypothesis**. Because repeated measurements on the same chicken may be correlated, the exact reference distribution requires independent, homoscedastic Gaussian errors; the displayed ordinary regression output by itself does not establish that assumption.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5J](../../5j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Taking logarithms of the [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md) gives

$$
S(\beta)=\sum_{i=1}^n v_i\left[\beta z_i-\log\left(\sum_{j:x_j\geq x_i}e^{\beta z_j}\right)\right].
$$

Differentiate each term, using the [chain rule](../../../../../../../chain-rule.md) for the logarithm:

$$
\boxed{S'(\beta)=\sum_{i=1}^n v_i\left[z_i-
\frac{\sum_{j:x_j\geq x_i}z_j e^{\beta z_j}}{\sum_{j:x_j\geq x_i}e^{\beta z_j}}\right].}
$$

This [score function](../../../../../../../informant-function.md) is the sum over failures of the observed covariate minus its current risk-weighted mean. Define that mean as $\overline z_\beta(x_i)$; observations with $v_i=0$ have no direct event term, although they occur in the relevant [risk sets](../../../../../../../risk-set.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

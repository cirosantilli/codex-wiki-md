<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The dispersion-one assumption is strongly contradicted by the preceding calculation. **Use the gamma analysis with estimated dispersion, namely the F table.** A failure to reject shape three does not establish that the true shape equals exactly three; retaining the estimated [dispersion parameter](../../../../../../dispersion-parameter.md) $0.3103711$ is appropriate.

In the [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md), a deviance reduction for $r$ extra coefficients is divided by $r\widehat\phi$ when dispersion is estimated. The approximate null calibration is $F_{r,57}$. For the type term, the null is that the two type contrasts vanish, against at least one nonzero contrast. The statistic is

$$
F=\frac{2.60027/2}{0.3103711}=4.1890,
$$

with approximate null distribution $F_{2,57}$ and [p-value](../../../../../../p-value.md) $0.02007$. For position, the null is that its coefficient vanishes after accounting for type; the statistic is

$$
F=\frac{0.27603}{0.3103711}=0.8894,
$$

with approximate null distribution $F_{1,57}$ and [p-value](../../../../../../p-value.md) $0.34963$. At 5% there is evidence that component type affects the expected failure time, and no significant additional position effect. The table is sequential: the type comparison is to the intercept-only model, while the position comparison adjusts for type. The individual gamma coefficient tests also suggest that type 3 accounts for the clearer type difference. The inverse [link function](../../../../../../link-function.md) means its positive contrast corresponds to a lower fitted mean failure time, holding position fixed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the difference as control minus intervention, positive for fewer deaths under intervention assignment. The observed difference per thousand is

$$
\widehat\Delta=1000\left(\frac{148}{30000}-\frac{123}{30000}\right)=\frac{25}{30}\simeq0.833.
$$

For independent [binomial distributions](../../../../../../binomial-distribution.md), its unpooled standard error per thousand is

$$
\widehat{\rm SE}=1000\sqrt{\frac{\widehat p_C(1-\widehat p_C)}{30000}+\frac{\widehat p_I(1-\widehat p_I)}{30000}}\simeq0.547.
$$

The approximate 95% [confidence interval](../../../../../../confidence-interval.md) is therefore

$$
\boxed{0.833\pm1.96(0.547)\simeq(-0.24,\ 1.91)\text{ fewer deaths per thousand}.}
$$

The rare-event Poisson standard error $\sqrt{148+123}/30$ gives almost the same interval. **A reduction of 1.5 per thousand is consistent with the data**, since it lies inside the interval. Zero also lies inside, so a nonzero benefit is not established at the two-sided 5% significance level. This does not establish equivalence or prove the proposed effect size, and cannot by itself establish [treatment contamination](../../../../../../treatment-contamination.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

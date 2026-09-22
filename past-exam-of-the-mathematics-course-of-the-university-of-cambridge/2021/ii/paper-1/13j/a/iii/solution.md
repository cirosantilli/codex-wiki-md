<h1 id="13j/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The additive model has four free [coefficients](../../../../../../../regression-coefficient.md): an intercept, two treatment contrasts, and one outcome contrast. The interaction model adds

$$
(3-1)(2-1)=2
$$

treatment-by-outcome [interaction term](../../../../../../../interaction-term.md), making six parameters for six cells. It is saturated, so the residual degrees of freedom fall from two to zero and the [likelihood-ratio test](../../../../../../../likelihood-ratio-test.md) has

$$
\boxed{6-4=2\text{ degrees of freedom}}.
$$

The deviance reduction is $44.48$, with p-value $2.194\times10^{-10}$. The [analysis of deviance for nested generalized linear models](../../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) therefore gives overwhelming evidence against a common outcome distribution across the three groups. The observed proportions and the negative treatment--Worse interactions show that both doses reduce the chance of worsening relative to Control, with a larger reduction for LD.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [13J](../../../13j.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

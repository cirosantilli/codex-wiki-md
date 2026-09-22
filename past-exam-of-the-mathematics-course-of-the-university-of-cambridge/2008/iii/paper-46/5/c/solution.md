<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under [proportional hazards](../../../../../../proportional-hazards-model.md), each coefficient is constant over event time. Examine the [Schoenfeld residuals](../../../../../../schoenfeld-residual.md), preferably [scaled Schoenfeld residuals](../../../../../../scaled-schoenfeld-residual.md), against time or a prespecified transformation such as log time, ranks or a fitted survival-time transformation. Plot a smooth trend and its uncertainty for each [covariate](../../../../../../covariate.md). Under the working model there should be no systematic residual-time association; a persistent trend suggests a time-varying coefficient. In a coefficient-scale plot that adds $\widehat\beta$ to the scaled residuals, the null trend is horizontal at the fitted coefficient.

A formal [proportional hazards assumption test](../../../../../../proportional-hazards-assumption-test.md) can add a time interaction, for example $\beta_r(t)=\beta_r+\theta_r g(t)$, and test $\theta_r=0$ using a score test with information adjusted for the fitted constant coefficients. The score contributions involve the Schoenfeld functions weighted by $g(t_j)$. One can test each [covariate](../../../../../../covariate.md) and use a joint global test for a vector of time-interaction coefficients. Such an association would be possible despite the unweighted residual sum being zero, so that fitted identity does not establish [proportional hazards](../../../../../../proportional-hazards-model.md).

**A systematic nonhorizontal coefficient trend or significant residual-time association is evidence against a constant [hazard ratio](../../../../../../hazard-ratio.md).** Failure to reject is compatible with the assumption, not proof of it. These diagnostics target the proportionality restriction; they do not by themselves verify [covariate](../../../../../../covariate.md) functional form or independence of the censoring mechanism.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

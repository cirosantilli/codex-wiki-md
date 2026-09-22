<h1 id="13j/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Equal LD and SD efficacy is equivalent to

$$
p_L=p_S,
$$

because both efficacy definitions use the same control probability. In this two-outcome table that is also equivalent to equality of the LD and SD log-odds interactions,

$$
H_0:\gamma_{LW}=\gamma_{SW}.
$$

The summary gives the two estimates and their individual [standard error](../../../../../../../standard-error.md), but a test of their difference needs

$$
\operatorname{Var}(\widehat\gamma_{LW}-\widehat\gamma_{SW})
=\operatorname{Var}(\widehat\gamma_{LW})
+\operatorname{Var}(\widehat\gamma_{SW})
-2\operatorname{Cov}(\widehat\gamma_{LW},\widehat\gamma_{SW}).
$$

The required [covariance](../../../../../../../covariance.md) is absent from the displayed table, so the two separate coefficient p-values cannot test equality.

Instead, fit the [equal-efficacy Poisson log-linear model](../../../../../../../equal-efficacy-poisson-log-linear-model.md). For example, create one indicator for a Worse outcome in either treated group:
```
r
data$treated_worse <- with(data, treatment != "Control" & outcome == "Worse")
fit_equal <- glm(count ~ treatment + outcome + treated_worse,
                 family = poisson, data = data)
anova(fit_equal, fit2, test = "LRT")
```
The reduced model has one common treated-versus-control outcome interaction, while retaining separate LD and SD main effects for their different group totals. The full model has two such interactions. Their [analysis of deviance for nested generalized linear models](../../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) is therefore a one-degree-of-freedom likelihood-ratio test of equal efficacy.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
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

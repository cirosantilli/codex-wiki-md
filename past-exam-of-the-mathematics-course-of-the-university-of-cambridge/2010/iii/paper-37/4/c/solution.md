<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The second [Poisson exposure model](../../../../../../poisson-exposure-model.md) allows each location its own baseline accident rate:

$$
Y_{it}\overset{\mathrm{ind}}\sim\operatorname{Poisson}(e_{it}e^{\alpha+\lambda_i+\beta t}),\qquad\lambda_1=0.
$$

The last equality is the [corner-point constraint](../../../../../../corner-point-constraint.md). The common after-to-before [incidence rate ratio](../../../../../../rate-ratio.md) remains $e^\beta$. This model is appropriate because the sites can have different background risks; treating those differences as unexplained Poisson variation made the first model fit poorly, with deviance $50.863$ on 14 [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md).

Adding seven location effects to the first fitted model reduces the deviance by $50.863-16.275=34.588$, which is large relative to $\chi^2_7$. The supplied sequential [analysis of deviance](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) reports a slightly different location contribution because it enters locations before the period indicator. The full model is much better but its deviance $16.275$ on 7 degrees of freedom still gives an approximate goodness-of-fit $p$-value $0.0227$. That suggests residual lack of fit or [overdispersion](../../../../../../overdispersion.md), although sparse accident counts make the asymptotic [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) approximate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

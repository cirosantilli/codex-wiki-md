<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There are two different effect scales in this [zero-inflated Poisson regression](../../../../../../../zero-inflated-poisson-regression.md). The count component describes the mean $\mu$ conditional on belonging to the susceptible component, including its possible zero outcomes. Its [logarithmic link function](../../../../../../../logarithmic-link-function.md) coefficients exponentiate to ratios of those conditional means. The zero component describes the structural-zero probability $\pi$; its logit coefficients exponentiate to [odds ratios](../../../../../../../odds-ratio.md), not probability ratios.

Holding the other covariates fixed, Centre B versus Centre A changes the susceptible count mean by the factor

$$
\boxed{e^{0.434635}=1.5444,}
$$

an increase of about $54.4\%$. It simultaneously multiplies the odds of being a structural zero by

$$
\boxed{e^{0.6715}=1.9571.}
$$

Thus Centre B is associated both with higher count intensity among susceptible patients and with greater odds of belonging to the never-at-risk class.

Use no personality disorder as the reference. For women, borderline disorder multiplies the susceptible count mean by $e^{-0.224673}=0.7988$, and other disorder multiplies it by $e^{-1.564576}=0.2092$. Because the count model has sex-by-disorder [interaction terms](../../../../../../../interaction-term.md), the corresponding male comparisons must add the interactions before exponentiating:

$$
\boxed{\begin{aligned}
RR_{\rm borderline,male}&=e^{-0.224673-0.240213}\approx0.6282,\\
RR_{\rm other,male}&=e^{-1.564576+1.462261}\approx0.9027.
\end{aligned}}
$$

These compare men with the stated disorder to otherwise comparable men without a disorder; the female comparisons use female reference patients. The interaction multipliers $0.7865$ and $4.3157$ alone are ratios of these sex-specific disorder ratios, not the overall male disorder effects.

In the zero component there is no sex-by-disorder interaction. Borderline and other disorders multiply the structural-zero odds relative to no disorder by **$0.4217$ and $0.5504$**, respectively, holding centre fixed; these comparisons are the same for both sexes in the fitted zero model.

The marginal mean is $E(Y)=(1-\pi)\mu$. Therefore none of these count multipliers alone is the population-average change in expected episodes when the same covariate also changes $\pi$. For a count coefficient change $b$ and zero-logit change $g$ from baseline zero predictor $\eta$, the marginal mean ratio is

$$
\boxed{RR_{\rm marginal}=e^b\frac{1+e^{\eta}}{1+e^{\eta+g}}.}
$$

For centre use $(b,g)=(0.434635,0.6715)$; for disorder use its sex-specific count contrast and its zero contrast. This is the [component and marginal effects in zero-inflated regression](../../../../../../../component-and-marginal-effects-in-zero-inflated-regression.md) distinction needed to interpret these results carefully.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

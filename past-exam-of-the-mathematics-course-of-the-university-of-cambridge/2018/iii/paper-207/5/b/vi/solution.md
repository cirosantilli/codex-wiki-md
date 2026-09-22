<h1 id="5/b/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Fit the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md) with the other explanatory variables, initially omitting the variable $z$ whose form is being assessed, and plot the resulting [martingale residuals](../../../../../../../martingale-residual.md) against $z$. Add a smooth trend, for example using a [cubic spline](../../../../../../../cubic-spline.md) or a local smoother. A systematic pattern indicates that $z$ affects the [hazard function](../../../../../../../hazard-function.md); the shape helps suggest a linear term, a transformation, or a nonlinear spline term in the log hazard.

Refit with the proposed form and inspect [martingale residuals](../../../../../../../martingale-residual.md) against $z$ again. Under an adequate functional form, their conditional mean should have no systematic trend, allowing for model fitting and the other covariates. Compare plausible alternative forms using the [partial likelihood](../../../../../../../partial-likelihood.md) and suitable model checks.

**Use the smoothed pattern to assess the covariate's functional form, rather than treating these residuals as normal regression errors.** [Martingale residuals](../../../../../../../martingale-residual.md) are asymmetric, bounded above by 1, and can be arbitrarily negative; the raw residual plot can therefore be misleading without smoothing. This diagnostic concerns the covariate form, and does not by itself test the [proportional hazards](../../../../../../../proportional-hazards-model.md) assumption.

## ↑ Ancestors (12)

1. [Vi](../vi.md)
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

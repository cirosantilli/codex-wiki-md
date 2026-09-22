<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The command `cox.zph` checks the [proportional hazards assumption test](../../../../../../../proportional-hazards-assumption-test.md) through time dependence of [scaled Schoenfeld residuals](../../../../../../../scaled-schoenfeld-residual.md). Under constant coefficients, their expected trend against transformed event time should be flat. A significant covariate-specific test would suggest that its coefficient varies with time; the global test checks the coefficients jointly.

The [p-values](../../../../../../../p-value.md) are $0.461$ for age, $0.538$ for gender and $0.882$ for group, with global $p=0.846$. Thus **these tests find no evidence against proportional hazards**. They do not prove the assumption, establish the correct age functional form, or test the censoring mechanism.

The separate diagnostic plot targets the broader fitted survival distribution. The code evaluates a fitted [cumulative hazard function](../../../../../../../cumulative-hazard-function.md) at each observed time and multiplies by the subject's fitted hazard multiplier, forming [Cox–Snell residuals](../../../../../../../cox-snell-residual.md):

$$
r_i=\widehat H_i(T_i)=\widehat H_{\mathrm{ref}}(T_i)\exp\{\widehat\eta_i\}.
$$

The curve returned without `newdata` by `survfit` is a reference-profile curve, not necessarily the all-zero-covariate baseline. The multiplier must use the same centering as that reference curve; the fitted linear predictors use the model's reference convention. With this consistency, $-\log\widehat S_{\mathrm{ref}}$ times the multiplier is the fitted subject-specific cumulative hazard.

Part (a) shows why complete transformed event times should be approximately unit exponential if the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md) is correct. The Q–Q plot compares ordered fitted residuals with an independent random exponential sample. Most points are near the diagonal, with some upper-tail departures, so it gives **no obvious indication of a gross distributional failure**. A random reference sample adds simulation noise, and estimated parameters and tied recorded times prevent this from being an exact distribution-free test.

Importantly, four observed times are censored. Their transformed times retain the censoring indicators and are not complete exponential observations. Simply plotting all $100$ residuals as uncensored therefore gives only a rough visual check. A more appropriate [Cox–Snell residual survival diagnostic](../../../../../../../cox-snell-residual-survival-diagnostic.md) fits a [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md) or [Nelson–Aalen estimator](../../../../../../../nelson-aalen-estimator.md) to $(r_i,D_i)$, retains the censoring flags, and checks whether the estimated cumulative hazard is close to $r$, equivalently whether estimated survival is close to $e^{-r}$. Taken together, the supplied checks are broadly compatible with the fitted model, while none resolves potentially [informative censoring](../../../../../../../informative-censoring.md) from giving up.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

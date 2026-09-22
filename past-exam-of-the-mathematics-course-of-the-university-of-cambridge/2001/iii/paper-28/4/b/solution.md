<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

These are separate data, so results from the randomized trial must not be carried over. First inspect the construction of the survival response: a command creating a [survival time](../../../../../../survival-time.md) object must pair follow-up in months with an event indicator, whose death/censoring coding should be checked explicitly. A censoring time is not an observed death time. Stratified product-limit fits would then summarize [Kaplan–Meier estimators](../../../../../../kaplan-meier-estimator.md) for the dose groups before adjusted regression.

If the fitted command is a [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md) with dose, sex and age, its specification is

$$
h(t\mid G,F,A)=h_0(t)\exp(\beta_GG+\beta_FF+\beta_AA).
$$

There is no separate intercept estimate because an intercept is absorbed into the unspecified baseline hazard $h_0$. With the stated coding, $e^{\beta_G}$ compares high-dose with low-dose death hazards at equal sex and age; $e^{\beta_F}$ compares female with male hazards at equal dose and age; $e^{\beta_A}$ is the hazard multiplier for a one-year age increase. A negative treatment coefficient would correspond to a lower fitted hazard under high dose. A [hazard ratio](../../../../../../hazard-ratio.md) is not a ratio of survival probabilities, nor directly a ratio of survival times. Under this model the survivor function is $S(t\mid x)=S_0(t)^{\exp(x^T\beta)}$.

The coefficient [standard errors](../../../../../../standard-error.md), Wald ratios and exponentiated [confidence intervals](../../../../../../confidence-interval.md) should be read together. The common large-sample interval for a coefficient's [hazard ratio](../../../../../../hazard-ratio.md) is

$$
\exp\{\widehat\beta\pm1.96\operatorname{se}(\widehat\beta)\}.
$$

Global likelihood-ratio, score and Wald tests assess the included slopes jointly; for exactly these three one-coefficient terms their reference degrees of freedom are three. They need not coincide in a small sample. The [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) uses the event risk sets; the fitted log-likelihood is not a full likelihood for an estimated baseline survival curve. The method for tied event times should be recorded.

Check the [proportional hazards](../../../../../../proportional-hazards-model.md) assumption using [scaled Schoenfeld residuals](../../../../../../scaled-schoenfeld-residual.md) and time trends; check the functional form of age, influential subjects and [independent censoring](../../../../../../independent-censoring.md). Dose-by-age or dose-by-sex [interaction terms](../../../../../../interaction-term.md) are scientifically possible but require enough information and a stated model comparison. Adjustment can alter a crude dose association, and the allocation mechanism here is not specified as randomized. **No coefficients, confidence limits, significance results, exact fitted calls or diagnostics for this dataset are recoverable without the output sheet.** The displayed model is an interpretation template, not a claim that it was the exact missing command.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

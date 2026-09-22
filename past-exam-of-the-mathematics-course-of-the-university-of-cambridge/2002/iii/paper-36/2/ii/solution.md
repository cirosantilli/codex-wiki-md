<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The family-history table contains $462$ men, of whom $160$ have the response present, giving an overall observed fraction $160/462=0.3463$. The unadjusted fractions are $96/192=0.5$ with a positive family history and $64/270=0.2370$ without one. Their crude [odds ratio](../../../../../../odds-ratio.md) is $(96/96)/(64/206)=3.219$; this is not the covariate-adjusted effect from the fitted [logistic regression](../../../../../../logistic-regression.md).

The full model has an intercept and nine slopes, hence $462-10=452$ residual degrees of freedom. The [binomial distribution](../../../../../../binomial-distribution.md) dispersion is fixed at one. Although the software labels coefficient-to-standard-error ratios as t values, here they are asymptotic normal [Wald statistics](../../../../../../wald-test.md), not statistics with an estimated Gaussian residual [variance](../../../../../../variance-split.md) and an exact Student reference. The full conditional coefficients provide evidence for tobacco, cholesterol, family history, behaviour score and age: their absolute Wald ratios are approximately $2.99,2.92,4.06,3.22,3.73$. The other four ratios are smaller in magnitude, especially alcohol at about $0.027$. These are conditional associations; a weak adjusted coefficient does not by itself establish absence of an underlying association, and [multicollinearity](../../../../../../multicollinearity.md) can affect the estimates.

The null [deviance](../../../../../../exponential-family-deviance.md) is $596.1084$ on $461$ degrees of freedom and the full [residual deviance](../../../../../../residual-deviance.md) is $472.14$ on $452$. Their difference $123.9684$ has a nominal nine-degree-of-freedom [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) reference for the nine slopes jointly. The absolute [residual deviance](../../../../../../residual-deviance.md) should not automatically be compared with $\chi^2_{452}$ for the reasons in part (i).

The shown [stepwise selection by the Akaike information criterion](../../../../../../stepwise-selection-by-the-akaike-information-criterion.md) follows a backward path. For individual binary observations the saturated [log-likelihood](../../../../../../log-likelihood.md) is zero, so

$$
\boxed{\operatorname{AIC}=D+2k},
$$

where $k$ includes the intercept. Removing a one-parameter term improves AIC exactly when the increased [deviance](../../../../../../exponential-family-deviance.md) is less than two. The successive deletions are alcohol, adiposity, blood pressure and obesity. The corresponding $(D,k,\operatorname{AIC})$ values are

$$
\begin{aligned}
&(472.1400,10,492.1400),\quad(472.1408,9,490.1408),\\
&(472.5490,8,488.5490),\quad(473.9799,7,487.9799),\\
&(475.6856,6,487.6856).
\end{aligned}
$$

At the final step, every remaining single-term deletion increases AIC. This is a local stopping condition of the search, not a proof that it found the best subset among all possible models. Obesity is retained for several steps because its successive deletion costs differ after the other terms are removed; the procedure does not simply sort the initial Wald ratios.

For the selected fit, write $H=1$ for positive family history and $H=0$ otherwise. The fitted linear predictor is

$$
\boxed{\widehat\eta=-6.446392+0.0803751\,\mathrm{tobacco}
+0.161991\,\mathrm{ldl}+0.908171H
+0.0371149\,\mathrm{typea}+0.0504598\,\mathrm{age},
\qquad\widehat p=\frac{e^{\widehat\eta}}{1+e^{\widehat\eta}}}.
$$

Holding the other predictors fixed, a unit increase multiplies the odds by $e^{\widehat\beta_j}$. In the same variable order, the unit [odds ratios](../../../../../../odds-ratio.md) are

$$
\boxed{1.084,\quad1.176,\quad2.480,\quad1.038,\quad1.052}.
$$

A ten-year age difference multiplies the fitted odds by $1.656$, and ten behaviour-score points by $1.449$. Family history has adjusted [odds ratio](../../../../../../odds-ratio.md) about $2.48$, with ordinary fitted-model $95\%$ [confidence interval](../../../../../../confidence-interval.md) $\exp(0.908171\pm1.96\times0.225603)\simeq[1.59,3.86]$. The intercept is the log odds at zero numerical covariates and absent family history; that extrapolated baseline is not a typical man's risk. Odds ratios are not risk ratios.

The selected model's residual degrees of freedom are $456$, consistent with its six coefficients. All five retained slopes have nominal normal-Wald $p$ values below $0.004$ in that model, but these tests and [confidence intervals](../../../../../../confidence-interval.md) do not incorporate the prior [model selection](../../../../../../model-selection.md). Its improvement over the intercept-only fit is $596.1084-475.6856=120.4228$ on five nominal degrees of freedom; it loses only $3.5456$ [deviance](../../../../../../exponential-family-deviance.md) units relative to the nine-slope fit while using four fewer parameters. Selection optimism remains relevant to predictive performance. Check possible nonlinear continuous-predictor effects, influential observations and clinically motivated interactions; assess out-of-sample discrimination and agreement of predicted [probabilities](../../../../../../probability.md) with observed frequencies by [cross-validation](../../../../../../cross-validation.md) or external data. The printed output alone does not supply those diagnostics, and the selected high-risk male population limits extrapolation to other populations. Nothing here establishes causal effects of these observational predictors.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the population as exposure regardless of whether a population-size category is also a covariate. Define a demographic factor with levels $\mathrm{Low}$ for at most 20%, $\mathrm{Medium}$ for $(20,30]$%, and $\mathrm{High}$ above 30%; define $H_{it}=\mathbf1_{\{P_{it}>250\}}$ if following the suggested population dichotomy. Treat village-size codes as a [categorical variable](../../../../../../categorical-variable.md), not equally spaced areas.

A candidate multivariate [Poisson generalized linear mixed model](../../../../../../poisson-generalized-linear-mixed-model.md) retains the random intercept and slope from part (c) and uses

$$
\begin{aligned}
\log\mu_{it}={}&\log P_{it}+\beta_0+\beta_1s+b_{0i}+b_{1i}s
+\theta_I I_i+\theta_M\mathbf1_{M_i=\mathrm{Medium}}
+\theta_H\mathbf1_{M_i=\mathrm{High}}\\
&+\gamma_2\mathbf1_{V_{it}=2}+\gamma_3\mathbf1_{V_{it}=3}
+\zeta H_{it}+\kappa_2 H_{it}\mathbf1_{V_{it}=2}
+\kappa_3 H_{it}\mathbf1_{V_{it}=3}.
\end{aligned}
$$

This specifies the suggested village-size-by-population interaction while keeping its main effects. One may add selected time-by-covariate interactions to explain slope heterogeneity, provided information from 32 clusters supports them. Compare continuous demographic and population formulations as a sensitivity analysis: categorization loses information, and the coefficient of a size category measures association beyond the already included exposure effect.

Fit models with the same likelihood convention and conditional distribution when comparing [Akaike information criteria](../../../../../../akaike-information-criterion.md); use joint fixed-effect [likelihood-ratio tests](../../../../../../likelihood-ratio-test.md), boundary-aware [parametric bootstrap](../../../../../../parametric-bootstrap.md) tests for random effects, residual diagnostics and village-level [cross-validation](../../../../../../cross-validation.md) to justify a parsimonious final model. Preserve interactions' main effects and report interval estimates from the final multivariate model, rather than interpreting separate univariate fits. For example, the adjusted inland-versus-coastal [rate ratio](../../../../../../rate-ratio.md) is $e^{\theta_I}$, while a medium-versus-small village ratio is $e^{\gamma_2+\kappa_2H}$; a Wald interval for that contrast uses the full coefficient [covariance matrix](../../../../../../covariance-matrix.md). Conditional time effects and standardized marginal predictions should be distinguished.

The displayed rows cannot identify this final model: population exceeds 250 in every displayed village-year, no large village is shown, and inland status is confounded with the identity of the two displayed villages. The complete 160-row file is needed for fitted effects, model selection, all-village plots and uncertainty. **No numerical best model or evidence of the specified covariate associations can honestly be reported from this excerpt.**

Finally, even a significant adjusted association with young-male percentage would not show that young males were involved in most incidents. This is the [ecological fallacy](../../../../../../ecological-fallacy.md), specifically that [aggregate composition does not identify offender composition](../../../../../../aggregate-composition-does-not-identify-offender-composition.md): the same village counts can be assigned to different individual age and sex groups without changing any observed aggregate predictor. Individual incident-level age, sex and involvement records are required to answer that last question. **The aggregate dataset cannot establish the claimed majority involvement.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

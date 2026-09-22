<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume a constant annual [force of infection](../../../../../force-of-infection.md) $\lambda>0$ across ages and calendar years. For independent sampled people with ages $a_i>0$ and binary results $y_i$, fit

$$
Y_i\sim\operatorname{Bernoulli}(p_i),\qquad p_i=1-e^{-\lambda a_i}.
$$

Applying the [complementary log-log link](../../../../../complementary-log-log-link.md) gives

$$
\begin{aligned}
\ln[-\ln(1-p_i)]&=\ln(\lambda a_i)\\
&=\beta_0+\ln a_i,\qquad\beta_0=\ln\lambda.
\end{aligned}
$$

Therefore fit a [binomial regression](../../../../../binomial-regression.md) with the [complementary log-log link](../../../../../complementary-log-log-link.md), an intercept, and **$\ln a_i$ as an offset with coefficient fixed at one**. Age is measured in years. An ordinary freely fitted coefficient of age, or even a freely fitted coefficient of $\ln a_i$, would describe a different exposure model. The annual [force of infection](../../../../../force-of-infection.md) estimate is

$$
\boxed{\widehat\lambda=e^{\widehat\beta_0}\ \text{year}^{-1}}.
$$

An infection-naive person's one-year infection probability is $1-e^{-\widehat\lambda}$, which is approximately $\widehat\lambda$ only when that rate is small.

The [log-likelihood](../../../../../log-likelihood.md) being maximized is, apart from constants,

$$
\ell(\beta_0)=\sum_i\left[y_i\ln\{1-\exp(-a_ie^{\beta_0})\}-(1-y_i)a_ie^{\beta_0}\right].
$$

A [confidence interval](../../../../../confidence-interval.md) for $\beta_0$ can be exponentiated to give a positive interval for $\lambda$. For groups of $n_j$ people at a common age $a_j$, use $Y_j\sim\operatorname{Binomial}(n_j,1-e^{-\lambda a_j})$ with the same [offset](../../../../../generalized-linear-model-offset.md). If an age band is broad, use individual ages or average $1-e^{-\lambda a}$ over the band's age distribution instead of treating its midpoint as exact. No numerical estimate is possible without the survey observations.

The biological interpretation assumes that [immunoglobulin G](../../../../../immunoglobulin-g.md) positivity records previous infection, persists over the relevant ages, and is not substantially produced by maternal antibodies or vaccination. These are conditions to check, rather than conclusions from the fitted curve. Use known-positive and known-negative serum controls to assess the assay threshold, and validate specificity against relevant other infections. Cross-reactive antibodies to other flaviviruses can produce positive [dengue virus](../../../../../dengue-virus.md) serology, so a positive result need not be a marker specific to [dengue virus](../../../../../dengue-virus.md) exposure.[IgG Tests: persistence after previous exposure and cross-reactivity with other flaviviruses](../../../../../serologic-tests-for-dengue-virus-by-the-centers-for-disease-control-and-prevention.md)

If independently established assay [diagnostic sensitivity](../../../../../diagnostic-sensitivity.md) and [diagnostic specificity](../../../../../diagnostic-specificity.md) are $Se$ and $Sp$, the observed positive probability is

$$
p_{i,\mathrm{obs}}=Se(1-e^{-\lambda a_i})+(1-Sp)e^{-\lambda a_i}.
$$

Use that observation model in the [binomial likelihood](../../../../../binomial-likelihood.md); it is generally no longer the simple intercept-plus-offset [complementary log-log link](../../../../../complementary-log-log-link.md) fit. With only the stated survey, one cannot freely estimate $Se$, $Sp$, antibody loss and an arbitrary infection history simultaneously. A single binary result also does not identify how many subsequent infections a person has experienced.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

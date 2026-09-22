<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Multiple imputation by chained equations](../../../../../../multiple-imputation-by-chained-equations.md) specifies one [conditional distribution](../../../../../../conditional-distribution.md) for each incomplete variable. In general, let $V_1,\ldots,V_q$ be the incomplete variables, $Z$ the fully observed predictors, and $\phi_j$ the parameters of a model $p_j(V_j\mid V_{-j},Z;\phi_j)$. The notation $V_{-j}$ means all variables except $V_j$. The models should respect each variable's support and contain the terms needed by the planned analysis.

First choose suitable models and initialise only the missing entries with admissible provisional values. One sweep updates $j=1,\ldots,q$ in turn. At update $j$, fit its model to records whose $V_j$ is observed, using the latest filled-in predictors. Draw

$$
\phi_j^*\sim p(\phi_j\mid V_{j,\mathrm{obs}},V_{-j}^{\mathrm{current}},Z),
\qquad
V_{j,\mathrm{mis}}^*\sim p_j(V_{j,\mathrm{mis}}\mid V_{-j}^{\mathrm{current}},Z;\phi_j^*).
$$

The first draw represents parameter uncertainty through a [Bayesian posterior](../../../../../../bayesian-posterior.md); the second represents residual uncertainty through a [posterior predictive distribution](../../../../../../posterior-predictive-distribution.md). Replace the missing entries with these draws, leaving every genuinely observed entry fixed. Repeat whole sweeps until the chain has settled, assessing traces, mixing and plausibility. Obtain $M$ completed datasets from independently initialised chains, or sufficiently separated draws after convergence. **Both parameter and missing-value uncertainty must be propagated; repeated deterministic prediction is not multiple imputation.**

Here use a [logistic regression](../../../../../../logistic-regression.md) for $C$ conditional on $P$, age and sex. For $P$, use an appropriate discrete count model conditional on $C$, age and sex, such as a suitably checked [negative binomial regression](../../../../../../negative-binomial-regression.md), allowing enough flexibility for skewness and nonlinear effects. Include interactions or transformations needed by the analysis in the imputation models. If condom use is structurally undefined for a record, preserve that applicability rule rather than treating it as ordinary [missing data](../../../../../../missing-data.md).

Impute the eligible survey information before discarding records solely because the observed $P$ is absent. In each completed dataset select its own $P>1$ records and fit the requested [logistic regression](../../../../../../logistic-regression.md). This allows a record with missing $P$ to contribute to the target group in some imputations and not others. Models must respect any known eligibility restrictions; if eligibility was independently known, use that information.

For a scalar [regression coefficient](../../../../../../regression-coefficient.md), let $\widehat Q_m$ be its estimate and $U_m$ its estimated [variance](../../../../../../variance-split.md) in completed dataset $m$. [Rubin's rules](../../../../../../rubin-s-rules.md) give

$$
\boxed{\overline Q=\frac1M\sum_m\widehat Q_m,\quad
\overline U=\frac1M\sum_m U_m,\quad
B=\frac1{M-1}\sum_m(\widehat Q_m-\overline Q)^2,\quad
T=\overline U+(1+M^{-1})B.}
$$

The [standard error](../../../../../../standard-error.md) is $\sqrt T$. Use the corresponding [multiple-imputation confidence interval](../../../../../../multiple-imputation-confidence-interval.md), rather than treating one completed dataset as fully observed. For vector coefficients replace the squared differences by outer products and $U_m$ by the covariance matrix. This combines within-imputation and between-imputation uncertainty.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

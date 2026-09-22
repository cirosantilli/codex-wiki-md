<h1 id="5/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a population question use a [population-averaged logistic model for repeated binary outcomes](../../../../../../../population-averaged-logistic-model-for-repeated-binary-outcomes.md). Code $z_i=1$ for the new treatment and $0$ for the control, with visit times $t_j=2j$ months for $j=1,2,3$. Let $w_{ij}=(1,z_i,x_i^T,t_j)^T$, $\gamma_M=(\alpha_M,\phi_M,\beta_M^T,\delta_M)^T$, and

$$
m_{ij}=P(Y_{ij}=1\mid z_i,x_i,t_j),\qquad\operatorname{logit}m_{ij}=w_{ij}^T\gamma_M.
$$

Different subjects are independent. Each response has a [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) with this marginal mean, but no independence of a subject's three responses is assumed. The linear time effect and absence of treatment-by-time [interaction](../../../../../../../interaction-statistics.md) are substantive mean assumptions; if inappropriate they can be replaced by time indicators and [interaction terms](../../../../../../../interaction-term.md).

For complete data, set $m_i=(m_{i1},m_{i2},m_{i3})^T$, $A_i=\operatorname{diag}(m_{ij}(1-m_{ij}))$, and $D_i=\partial m_i/\partial\gamma_M^T=A_iW_i$, where $W_i$ has rows $w_{ij}^T$. A working exchangeable [correlation matrix](../../../../../../../correlation-matrix.md) has unit diagonal and off-diagonal value $\rho\in(-1/2,1)$; set $V_i=A_i^{1/2}C(\rho)A_i^{1/2}$. The [generalized estimating equation](../../../../../../../generalized-estimating-equation.md) is

$$
\sum_iD_i^TV_i^{-1}(Y_i-m_i)=0.
$$

With correct means and independent subjects, a positive-definite working [covariance matrix](../../../../../../../covariance-matrix.md) and regularity give consistency even if the working correlation is wrong. Write $H=\sum_iD_i^TV_i^{-1}D_i$ and $u_i=D_i^TV_i^{-1}(Y_i-m_i)$. The fitted subject-level [sandwich covariance matrix](../../../../../../../sandwich-covariance-matrix.md) is

$$
\widehat{\operatorname{Var}}(\widehat\gamma_M)=H^{-1}\left(\sum_i u_iu_i^T\right)H^{-1},
$$

evaluated at the estimates. This inference is asymptotic in the number of independent subjects, not the number of visits.

For the actual incomplete data, define $R_{ij}=1$ if visit $j$ is observed, with $R_{i0}=1$ and monotone dropout. Let $\mathcal H_{i,j-1}$ contain treatment, baseline [covariates](../../../../../../../covariate.md) and responses observed before visit $j$. Under sequential [missing at random](../../../../../../../missing-at-random.md), specify

$$
q_{ij}=P(R_{ij}=1\mid R_{i,j-1}=1,\mathcal H_{i,j-1}),\qquad \rho_{ij}=\prod_{k=1}^j q_{ik}>0.
$$

The assumption is that the retention decision, conditional on this history, does not additionally depend on unseen current or future outcomes. Fit the $q_{ij}$, for example by visit-specific [logistic regressions](../../../../../../../logistic-regression.md). A simple valid choice uses working independence and the [inverse-observation-weighted estimating equations for longitudinal dropout](../../../../../../../inverse-observation-weighted-estimating-equations-for-longitudinal-dropout.md):

$$
\boxed{\sum_i\sum_{j=1}^3 w_{ij}\frac{R_{ij}}{\rho_{ij}}(Y_{ij}-m_{ij})=0.}
$$

Terms with $R_{ij}=0$ are zero and require no missing response. Given the full response vector, sequential [missing at random](../../../../../../../missing-at-random.md) makes $\mathbb E(R_{ij}/\rho_{ij}\mid Y_i,z_i,x_i)=1$. Consequently the weighted score has the same [expectation](../../../../../../../expected-value.md) as the complete-data score, proving its mean-zero property. Correct retention probabilities, positivity and a correctly specified marginal mean are required. Use cluster-robust uncertainty, accounting for fitted retention-model coefficients, or resample entire subjects and refit both models. Under [missing completely at random](../../../../../../../missing-completely-at-random.md), the simpler unweighted observed-response [GEE](../../../../../../../generalized-estimating-equation.md) can suffice; ordinary unweighted [GEE](../../../../../../../generalized-estimating-equation.md) is not valid under arbitrary history-dependent [missing at random](../../../../../../../missing-at-random.md).

The treatment coefficient gives a population conditional-on-baseline [odds ratio](../../../../../../../odds-ratio.md) $e^{\phi_M}$ at each visit. To communicate an absolute population treatment benefit, standardize predicted [probabilities](../../../../../../../probability.md) over the full baseline population, rather than only completers:

$$
\widehat p_z(t)=\frac1m\sum_i\operatorname{logit}^{-1}(\widehat\alpha_M+\widehat\phi_M z+\widehat\beta_M^Tx_i+\widehat\delta_M t),\qquad \widehat p_1(t)-\widehat p_0(t).
$$

A causal reading additionally uses the [randomized controlled trial](../../../../../../../randomized-controlled-trial.md) assignment, consistency of the treatment definition, no interference and the dropout assumptions; the statistical model alone does not supply those conditions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Ii](../../ii.md)
3. [5](../../../5.md)
4. [Paper 38](../../../../paper-38-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

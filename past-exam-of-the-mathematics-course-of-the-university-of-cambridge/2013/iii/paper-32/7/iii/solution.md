<h1 id="7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At each event time, a [Schoenfeld residual](../../../../../../schoenfeld-residual.md) is the observed event covariate minus its risk-set weighted mean:

$$
r_j=z_{i(j)}-\overline z(\widehat\beta,t_j),\qquad
\overline z(\beta,t)=\frac{\sum_{i\in R(t)}z_ie^{z_i^{\mathsf T}\beta}}
{\sum_{i\in R(t)}e^{z_i^{\mathsf T}\beta}}.
$$

Under a correct constant-coefficient model, these event-time residuals have no systematic time trend. Plot [scaled Schoenfeld residuals](../../../../../../scaled-schoenfeld-residual.md) against time or a prespecified transformation such as log time, with smooth curves and uncertainty bands. Depending on the plotting convention, adding the fitted coefficient produces an estimate of $\beta_k(t)$; a horizontal curve then supports a constant coefficient, while a clear trend suggests violation. Examine sparse late follow-up with its wider uncertainty.

Formal tests can use residual-time association or a [proportional-hazards time interaction](../../../../../../proportional-hazards-time-interaction.md) extension $\beta_k(t)=\beta_k+\gamma_kg(t)$, testing $\gamma_k=0$ jointly for a multi-parameter factor and globally across covariates. Evaluate $z_kg(t)$ at each current event/risk-set time: multiplying a baseline variable by that person's eventual observed follow-up time would use outcome information and would not be the intended time-dependent model. A nonsignificant test with limited information does not establish proportionality.

For categorical groups, approximately parallel empirical log-minus-log survival curves provide another check, because proportional hazards imply $\log[-\log S(t\mid z)]=z^{\mathsf T}\beta+\log H_0(t)$. Use observed group curves, not fitted proportional-hazards curves that are parallel by construction, and recognize possible confounding by other variables. If a violation is real, consider stratifying on a categorical nuisance variable, adding an explicitly time-varying effect, or choosing another survival-model family. Stratification allows separate [baseline hazards](../../../../../../baseline-hazard.md) but sacrifices a single estimated [hazard ratio](../../../../../../hazard-ratio.md) for that stratification variable. **Do not force a constant coefficient merely to preserve the original model label**; describe the time pattern or limit the interpretation of the constant summary.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

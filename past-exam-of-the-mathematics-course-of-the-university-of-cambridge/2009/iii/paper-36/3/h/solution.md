<h1 id="3/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Use [conditional versus marginal posterior predictive checks](../../../../../../conditional-versus-marginal-posterior-predictive-checks.md) to replicate new plates, rather than recycling the fitted plate effects. For each joint [posterior](../../../../../../bayesian-posterior.md) draw of $(\alpha,\beta,\gamma,\tau)$, draw fresh independent $\lambda_{ij}^{\mathrm{rep}}\sim N(0,\tau^2)$ and then

$$
Y_{ij}^{\mathrm{rep}}\sim\operatorname{Poisson}
\left(\exp\{\alpha+\beta\log(x_i+10)+\gamma x_i+\lambda_{ij}^{\mathrm{rep}}\}\right).
$$

Use the same doses and three-plate design, giving the [posterior predictive distribution](../../../../../../posterior-predictive-distribution.md) for repeated experiments. Compare observed dose means and their trend, the high-dose downturn, within-dose spreads, and outliers with the replicated curves and intervals. For example compare a discrepancy

$$
T(y;\psi)=\sum_i\frac{(\overline y_i-m_i)^2}{[m_i+m_i^2(e^{\tau^2}-1)]/3},
\qquad m_i=e^{\eta_i+\tau^2/2},
$$

with $T(y^{\mathrm{rep}};\psi)$ draw by draw. The resulting posterior predictive tail fraction or graphical rank assesses whether the observed trend is unusual under this model. **Fresh plate effects are needed to assess the population dose-response assumption.** Reusing the fitted effects would mainly check the conditional sampling layer and could hide systematic departures from the proposed curve.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

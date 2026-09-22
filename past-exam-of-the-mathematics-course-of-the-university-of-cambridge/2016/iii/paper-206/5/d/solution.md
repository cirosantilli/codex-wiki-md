<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [backfitting algorithm](../../../../../../backfitting-algorithm.md) to alternate conditional updates of the two additive functions. Initialize $\alpha=\overline Y$ and both centered function vectors at zero. With $S_e,S_d$ the [smoothing matrices](../../../../../../smoothing-matrix.md) for the chosen experience and education spline penalties, one cycle is

$$
r_e=Y-\alpha\mathbf1-f_d^{\mathrm{old}},\qquad
\widetilde f_e=S_er_e,\qquad
f_e^{\mathrm{new}}=\widetilde f_e-\overline{\widetilde f_e}\mathbf1,
$$

followed by

$$
r_d=Y-\alpha\mathbf1-f_e^{\mathrm{new}},\qquad
\widetilde f_d=S_dr_d,\qquad
f_d^{\mathrm{new}}=\widetilde f_d-\overline{\widetilde f_d}\mathbf1.
$$

The centering transfers any constant component to the intercept; update $\alpha$ to the mean of $Y-f_e-f_d$ if necessary, which is $\overline Y$ under the stated constraints. Repeat until changes in the functions or objective are negligible. Each function is estimated by smoothing its [partial residual](../../../../../../partial-residual.md), namely the response after subtracting all other currently fitted terms.

For fixed penalties these updates are block minimizations of

$$
\|Y-\alpha\mathbf1-f_e-f_d\|^2
+\lambda_e\int(f_e'')^2+\lambda_d\int(f_d'')^2,
$$

subject to the centering constraints. Each step cannot increase the objective; with identifiable additive terms and a positive-definite constrained quadratic, [backfitting](../../../../../../backfitting-algorithm.md) converges to its unique minimizer. Highly dependent predictors can make the decomposition poorly identified or slow convergence. The Gaussian identity-link model needs these least-squares updates directly; non-Gaussian [generalized additive models](../../../../../../generalized-additive-model.md) use weighted backfitting inside [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md). The package implementation also separates each spline's unpenalized linear component from its nonlinear component, giving the two ANOVA tables displayed in part (e).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

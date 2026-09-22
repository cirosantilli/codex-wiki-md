<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both fits use the Gaussian [generalized additive model](../../../../../../generalized-additive-model.md)

$$
Y_i=\alpha+f_e(e_i)+f_d(d_i)+\varepsilon_i,\qquad
\varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2),
\qquad\sum_i f_e(e_i)=\sum_i f_d(d_i)=0,
$$

where $e_i$ is experience and $d_i$ education. Centering makes the additive decomposition identifiable. No experience-education [interaction term](../../../../../../interaction-term.md) is included.

The first fit uses [local linear regression](../../../../../../local-linear-regression.md) for each term. `span=1` includes all observations in each nearest-neighbour neighbourhood, but distance weights and a moving target still vary: it does not make the fit exactly a global straight line. The second uses [cubic smoothing splines](../../../../../../cubic-smoothing-spline.md), with separate tuning values `spar=0.8` and `spar=1.2`. Increasing `spar` increases the curvature penalty and smooths more; `spar` is a monotone tuning parametrization, not the numerical $\lambda$ in part (b). The relation depends on the predictor scaling and design.

The plotted experience effect is increasing in both fits. The local fit gives a broadly smooth, nearly linear rise; the spline fit follows more of the steep low-experience rise and subsequent flattening, especially near the lower boundary. Education has a weaker increasing effect. The local estimate shows some curvature, while the spline fit at `spar=1.2` is closer to a straight line. **The clearest difference is the amount of smoothing and the experience curvature, rather than opposite effect directions.** These are centered partial-effect plots with [partial residuals](../../../../../../partial-residual.md), not scatterplots of wage against each predictor alone.

A smaller local span would allow the first fit to capture more experience curvature. A moderately smaller education `spar` could reveal nonlinear detail suppressed in the second fit; its small but significant nonparametric component in part (e) supports checking that possibility. Do not tune solely to follow every point, especially at sparse boundaries. Compare candidate spans or separate spline penalties using [cross-validation](../../../../../../cross-validation.md) or [generalized cross-validation](../../../../../../generalized-cross-validation.md); increase smoothing if flexible fits introduce unsupported wiggles. See the documented monotone `spar`–penalty convention at [https://stat.ethz.ch/R-manual/R-patched/library/stats/html/smooth.spline.html.](https://stat.ethz.ch/R-manual/R-patched/library/stats/html/smooth.spline.html.)

## ↑ Ancestors (11)

1. [C](../c.md)
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

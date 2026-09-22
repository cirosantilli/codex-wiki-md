<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For each plate use its conditional fitted intensity, including the fitted [random effect](../../../../../../random-effect.md). At a [posterior](../../../../../../bayesian-posterior.md) draw $s$ form the [Pearson residual](../../../../../../pearson-residual.md)

$$
\boxed{r_{ij}^{(s)}=\frac{y_{ij}-\mu_{ij}^{(s)}}{\sqrt{\mu_{ij}^{(s)}}}.}
$$

A simpler plot uses $\widehat\mu_{ij}$ in this expression, but posterior draws also display uncertainty in the fitted values. Look for residuals centred around zero, unexpectedly large tails or isolated outliers, and patterns with dose, fitted intensity or plate grouping. For known conditional parameters the [Poisson distribution](../../../../../../poisson-distribution.md) gives mean zero and variance one for this residual; approximate normality is reasonable only at adequate count sizes. Fitting the same data and estimating latent effects changes its calibration, so compare the diagnostics with residuals from conditional [posterior predictive checks](../../../../../../posterior-predictive-check.md), rather than treating them as independent exact standard normals.

This checks the plate-level Poisson sampling layer given the effects and can reveal remaining unmodelled variation. It does not by itself establish the population dose-response curve: fitted plate effects can absorb departures from that curve.

## ↑ Ancestors (11)

1. [G](../g.md)
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

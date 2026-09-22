<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The command fits a Gaussian [generalized additive mixed model](../../../../../../generalized-additive-mixed-model.md)

$$
\boxed{Y_{ij}=\alpha+s(t_{ij})+b_jt_{ij}+\varepsilon_{ij},\qquad b_j\overset{\rm iid}{\sim}N(0,\tau^2),\quad \varepsilon_{ij}\overset{\rm iid}{\sim}N(0,\sigma^2).}
$$

The population growth curve $s$ is a centered [penalized regression spline](../../../../../../penalized-regression-spline.md) with a cubic regression basis. The incubator term remains a [random slope](../../../../../../random-slope.md) without a [random intercept](../../../../../../random-intercept.md), because `~0+hours` removes the intercept. A population linear component is allowed within the smooth's unpenalized part; curvature is penalized rather than being required.

A `gamm` fit returns a list with `gam` and `lme` components. Plot the population smooth and pointwise uncertainty bands with
```
plot(fly.model2$gam, se=TRUE, residuals=TRUE)
```
Inspect whether the fitted curve departs materially from an [affine function](../../../../../../affine-function.md), particularly in regions supported by observations. The [effective degrees of freedom](../../../../../../effective-degrees-of-freedom.md) near one suggest that the penalization has selected an approximately linear centered smooth. Bands and partial residuals help distinguish convincing curvature from noisy deviations, although pointwise bands are not a simultaneous test of linearity. A formal comparison would need to account for both smoothing selection and the incubator dependence. **The smooth plot tests the visual plausibility of a common straight growth curve while retaining incubator-specific slope variation.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

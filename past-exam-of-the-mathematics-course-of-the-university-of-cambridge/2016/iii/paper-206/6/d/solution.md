<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The comparison removes the [random slope](../../../../../../random-slope.md) and tests $H_0:\tau_1^2=0$ against $H_1:\tau_1^2>0$, while retaining the same fixed intercept and slope. A variance cannot be negative, so zero is a boundary point of the parameter space. The regular [Wilks theorem](../../../../../../wilks-theorem.md) assumptions behind an ordinary $\chi^2_1$ [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) fail. Consequently the default chi-squared [p-value](../../../../../../p-value.md) from `anova` is not reliably calibrated for this [variance-component likelihood-ratio test at a boundary](../../../../../../variance-component-likelihood-ratio-test-at-a-boundary.md). This is different from the fixed-slope test in part (c). The reference to `strength_model1` means the earlier object `strength_model`; no separate model 1 object was defined.

A useful alternative is a [parametric bootstrap](../../../../../../parametric-bootstrap.md). Fit the null random-intercept model, then simulate data on the actual predictor values and furnace grouping by generating null intercept effects and observation errors from its fitted Gaussian distribution. Refit null and alternative models to each simulated dataset using the same likelihood method and compute the same likelihood-ratio statistic. If $T_{\mathrm{obs}}$ is the observed statistic, estimate its upper-tail probability by

$$
\boxed{\widehat p=\frac{1+\sum_{b=1}^{B}\mathbf1_{\{T_b\ge T_{\mathrm{obs}}\}}}{B+1}.}
$$

This incorporates the zero-variance boundary and the actual small group count. It is a fitted-null simulation approximation because nuisance parameters are estimated, not a universally exact test. Since both models have the same fixed-effect space, a similarly calibrated restricted-likelihood statistic is also possible. Under suitable asymptotics for a single identifiable added [variance component](../../../../../../variance-component.md) the familiar limiting law is $\tfrac12\chi^2_0+\tfrac12\chi^2_1$, but using the bootstrap avoids relying on that approximation with only three groups. There is no supplied statistic or calibrated bootstrap result here from which to decide whether the slope variance is required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

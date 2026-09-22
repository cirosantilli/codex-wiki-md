<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

With Control as the reference group, the fitted [normal linear model](../../../../../normal-linear-model.md) has mean

$$
\mathbb E[\mathrm{Weight}]
=\beta_0+\beta_{\rm Time}t+\beta_{\rm Treat}I_{\rm Treat}
+\beta_{\rm Int}tI_{\rm Treat}+\text{cage effect}.
$$

Thus the control-group rate is $\beta_{\rm Time}$, while the treatment-group rate is $\beta_{\rm Time}+\beta_{\rm Int}$. The estimates are

$$
\boxed{\widehat{\text{control slope}}=-0.006023,}
$$

and

$$
\boxed{\widehat{\text{treatment slope}}
=-0.006023-0.173515=-0.179538}
$$

weight units per day. The control slope has $t=-0.477$ and $p=0.63334$, so **there is no statistically significant evidence of weight loss over time in the control group** at conventional [significance levels](../../../../../significance-level.md).

The plotted [regression residuals](../../../../../regression-residual.md) for each mouse form smooth time patterns rather than an unstructured cloud: nearby observations on the same mouse have similar residuals, and the mice also show persistent individual offsets. This is strong evidence of [autocorrelation](../../../../../autocorrelation.md) and omitted mouse-level variation. The ordinary linear model treats all 400 measurements as independent after accounting for cage, so it commits [pseudoreplication](../../../../../pseudoreplication.md) and will generally underestimate the coefficient [standard errors](../../../../../standard-error.md). The reported $t$-tests and $p$-values should therefore **not be trusted**. A [random-intercept linear mixed model](../../../../../random-intercept-linear-mixed-model.md) with a within-mouse correlation structure would respect the repeated-measures design.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

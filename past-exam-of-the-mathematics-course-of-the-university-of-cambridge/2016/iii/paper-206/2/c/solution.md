<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $s_i$ be sunny days and $l_i$ latitude. The [R linear-model formula](../../../../../../r-linear-model-formula.md) expands to a [normal linear model](../../../../../../normal-linear-model.md) with both main effects and their [interaction term](../../../../../../interaction-term.md):

$$
Y_i=\beta_0+\beta_ss_i+\beta_ll_i+\beta_{sl}s_il_i+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The fitted conditional mean is

$$
\boxed{\widehat\mu_i=1.619+0.01403s_i+0.01438l_i-4.872\times10^{-6}s_il_i.}
$$

The residual [standard error](../../../../../../standard-error.md) is $0.2836$, giving the usual [variance](../../../../../../variance-split.md) estimate $s^2=0.08042896$, and $n=96+4=100$.

The estimated [interaction term](../../../../../../interaction-term.md) is tiny relative to its [standard error](../../../../../../standard-error.md): $t=-0.103$ and the two-sided [p-value](../../../../../../p-value.md) is $0.91811$. **A sensible initial simplification is to remove the interaction and refit an additive linear model**, `lm(energy ~ sunny + latitude)`. Both main effects are significant in the supplied fit, and should initially be retained. Do not simply copy their old coefficient estimates into the new fit: removing a design column generally changes all estimates. Centering predictors makes intercepts and main-effect interpretations more useful, but does not change the fitted surface. The [Box–Cox transformation](../../../../../../box-cox-transformation.md) in part (d) suggests a further response-scale improvement; after changing the response scale, reassess the interaction and diagnostics.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

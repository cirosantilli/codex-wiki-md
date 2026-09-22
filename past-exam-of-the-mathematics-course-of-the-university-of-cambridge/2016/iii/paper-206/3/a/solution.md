<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The initial [Poisson regression](../../../../../../poisson-regression.md) contains altitude, temperature, and their [interaction term](../../../../../../interaction-term.md), with a [logarithmic link function](../../../../../../logarithmic-link-function.md). Its interaction [Wald test](../../../../../../wald-test.md) has $p=0.521927$, suggesting removal of that term while initially preserving both main effects. The resulting additive model has a negligible temperature effect ($p=0.874$), suggesting a second simplification to altitude alone. The nested [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) gives the same provisional decisions: deviance increases are $83.326-82.916=0.410$ and $83.351-83.326=0.025$, each for one removed coefficient, with approximate $\chi^2_1$ upper-tail probabilities $0.522$ and $0.874$. The [Akaike information criterion](../../../../../../akaike-information-criterion.md) also decreases at each step.

For independent island counts the final proposed model is

$$
Y_i\sim\operatorname{Poisson}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_aa_i,
$$

with fitted relation

$$
\boxed{\widehat\mu(a)=\exp(3.24926+0.01898a).}
$$

This is an exponential mean relation on the count scale, not a linear relation between count and altitude. One additional metre multiplies the fitted expected count by $e^{0.01898}\approx1.01916$. The null model's insignificance of individual main effects in the interaction fit does not require discarding every predictor: correlated design columns can make those conditional tests imprecise. These reductions concern relative mean complexity under the working [Poisson regression](../../../../../../poisson-regression.md); the large residual deviance in all three models warns that their variance or mean assumptions still need investigation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

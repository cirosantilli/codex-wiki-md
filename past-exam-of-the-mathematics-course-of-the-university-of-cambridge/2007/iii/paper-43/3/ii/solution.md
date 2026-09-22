<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The null model uses one parameter, the day model uses nine, and there are $27$ grouped observations. The four missing entries, in their table order, are therefore

$$
\boxed{26,\qquad8,\qquad495.6308-32.7945=462.8363,\qquad18.}
$$

The test of no day effect is $H_0:\alpha_2=\cdots=\alpha_9=0$. The nominal binomial [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) statistic is $\Delta D=462.8363$, compared asymptotically with $\chi_8^2$. Its nominal $p$-value is about $6.6\times10^{-95}$, so the common-probability model is decisively inadequate relative to the day model. The fitted probabilities in (i) show substantial differences between days, with days 1 and 7 much higher than days 3 and 8.

However, relative improvement does not establish absolute fit. The day model's [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) compares $D=32.7945$ with $\chi_{18}^2$, giving $p\simeq0.0177$. The counts are large enough for this approximation to be reasonable. Thus at $5\%$ the day-specific binomial model still shows lack of fit. Among the two printed models it is preferred, but it should not be regarded as a fully satisfactory final model.

The residual scale estimate $D/18\simeq1.822$ suggests [overdispersion](../../../../../../overdispersion.md). Directly computing the Pearson statistic from the day means gives

$$
X^2=\sum_{i,j}\frac{(Y_{ij}-400\widehat p_i)^2}{400\widehat p_i(1-\widehat p_i)}\simeq32.70675,\qquad X^2/18\simeq1.81704.
$$

This corroborates extra dish variation rather than the nominal binomial [variance](../../../../../../variance-split.md). Dish heterogeneity or dependence among cells in a dish can produce such variation. Residual checks and a [quasibinomial regression](../../../../../../quasibinomial-regression.md) or an explicit model for dish heterogeneity are sensible refinements. Allowing dispersion of this moderate magnitude would enlarge [standard errors](../../../../../../standard-error.md) but would not plausibly remove the very large day effect. **Retain day effects, while accounting for the remaining extra-binomial variation.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

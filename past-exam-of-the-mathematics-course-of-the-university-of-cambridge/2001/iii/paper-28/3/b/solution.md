<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [normal linear model](../../../../../../normal-linear-model.md) with $n$ fixed observations and $p$ mean coefficients, maximizing over the error variance gives $\widehat\sigma^2=\operatorname{RSS}/n$. The maximized negative twice log-likelihood is $n\log(\operatorname{RSS}/n)$ plus a constant common to the candidate models. Counting the variance as another parameter adds the same penalty two to every model, so the stated criterion is equivalent for comparing them:

$$
\operatorname{AIC}=n\log(\operatorname{RSS}/n)+2p.
$$

The [Akaike information criterion](../../../../../../akaike-information-criterion.md) balances fit against parameter count; smaller values are preferred. It does not compare models using different response scales or different sets of observations without further adjustment.

[Stepwise selection by the Akaike information criterion](../../../../../../stepwise-selection-by-the-akaike-information-criterion.md) compares allowed one-term additions and deletions, takes a change lowering the criterion, and repeats until no allowed change improves it. The search direction, initial fit and lower/upper scopes matter. A displayed no-change row represents the current model. The term degrees of freedom show how many coefficients a change removes, the residual sum reflects its fit, and the AIC column determines the selected move. The search is greedy, not a guarantee of the best subset over the entire model space. The software's scope and direction conventions are documented in [https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/stepAIC.html](https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/stepAIC.html) .

Deleting $q$ coefficients changes the criterion by

$$
\Delta\operatorname{AIC}=n\log\frac{\operatorname{RSS}_{\mathrm{reduced}}}{\operatorname{RSS}_{\mathrm{full}}}-2q.
$$

Thus the [AIC deletion threshold in a normal linear model](../../../../../../aic-deletion-threshold-in-a-normal-linear-model.md) is

$$
\boxed{\operatorname{RSS}_{\mathrm{reduced}}/\operatorname{RSS}_{\mathrm{full}}<e^{2q/n}.}
$$

For a single coefficient, its [partial F-test](../../../../../../partial-f-test-for-nested-linear-models.md) statistic must be below $(n-p)(e^{2/n}-1)$ for AIC to favor deletion. At the full 47-observation, 16-coefficient fit this is approximately $1.348$, corresponding to $|t|<1.161$. Therefore AIC selection is not equivalent to retaining only coefficients with a conventional five-percent p-value.

The final model should be described by its retained terms, signs, conditional effect sizes, uncertainty, residual diagnostics and prediction behavior. A coefficient that survives selection need not identify a causal mechanism, and its ordinary final-model p-value ignores the preceding search. Stability under [bootstrap](../../../../../../bootstrapping-statistics.md) resampling and predictive [cross-validation](../../../../../../cross-validation.md) are useful. **The absent search trace and final model prevent identifying the actual deletion sequence, final predictors, coefficients, RSS or AIC.** The given starting name does not specify any of those facts.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

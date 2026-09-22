<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The commands read the 52 cell values into a vector and build the matching two-factor layout. In `expand.grid(country, goods)` the first [factor](../../../../../regression-factor.md) varies fastest, so the four countries are listed successively within each goods category. This matches row-by-row reading of the displayed table. Converting `Goods` to a [factor](../../../../../regression-factor.md) is essential: its labels identify 13 categories and are not a quantitative trend. `Country` supplies the other categorical [factor](../../../../../regression-factor.md). The summaries suppress coefficient correlations, not coefficient [standard errors](../../../../../standard-error.md).

The first fit is the additive [two-factor normal linear model](../../../../../two-factor-normal-linear-model.md)

$$
Y_{gc}=\mu+a_g+b_c+\varepsilon_{gc},\qquad
\varepsilon_{gc}\text{ independent }N(0,\sigma^2),\qquad a_1=b_{\mathrm{UK}}=0.
$$

There are $1+12+3=16$ free coefficients and $52-16=36$ residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). This is [two-way analysis of variance](../../../../../two-way-analysis-of-variance.md) without an [interaction term](../../../../../interaction-term.md). For this complete balanced layout, [ordinary least squares](../../../../../ordinary-least-squares.md) gives

$$
\widehat Y_{gc}=\overline Y_{g\cdot}+\overline Y_{\cdot c}-\overline Y_{\cdot\cdot},\qquad
\widehat a_g=\overline Y_{g\cdot}-\overline Y_{1\cdot},\qquad
\widehat b_c=\overline Y_{\cdot c}-\overline Y_{\cdot\mathrm{UK}}.
$$

These formulas follow from the row- and column-sum normal equations: fitted row and column totals equal their observed totals. The balanced-design coefficient [standard errors](../../../../../standard-error.md) are $s\sqrt{2/4}$ for a goods contrast, $s\sqrt{2/13}$ for a country contrast, and $s\sqrt{1/4+1/13-1/52}$ for the reference-cell intercept. These yield the common contrast [standard errors](../../../../../standard-error.md) and the different intercept [standard error](../../../../../standard-error.md) in each summary. In particular the intercept is the fitted Software–UK value, not the grand mean or the observed Software–UK entry.

Thus the first intercept predicts $149.8269$ million euros for Software in the UK. The Books coefficient adds $254.7$ million euros to the fitted value in any country, relative to Software; every other goods coefficient has this same arithmetic-difference interpretation. The country coefficients subtract $193.7$, $57.0308$ and $97.3769$ million euros from the UK prediction for France, Germany and the rest of Europe respectively, regardless of goods. The model therefore assumes common absolute country differences across goods categories. For Software–France its prediction is

$$
149.8269-193.7=-43.8731\text{ million euros},
$$

which is impossible for positive spending and indicates a limitation of this additive original-scale specification.

The [residual standard error](../../../../../residual-standard-error.md) is $80.98$ million euros, obtained from $s^2=\operatorname{RSS}/36$; direct calculation gives $\operatorname{RSS}=236088.7435$. Each coefficient's printed statistic is $\widehat\theta/\operatorname{se}(\widehat\theta)$, with a $t_{36}$ reference distribution under this [normal linear model](../../../../../normal-linear-model.md). The two-sided [p-values](../../../../../p-value.md) compare each goods category with Software, or each other country with the UK, after adjustment for the other [factor](../../../../../regression-factor.md). For example France and the rest of Europe differ significantly from the UK at 5%, but Germany does not. The raw-scale significant goods differences are Books, Clothing, Electronic Goods, Groceries and Leisure Travel; these are individual reference-level comparisons, not an overall test of the goods [factor](../../../../../regression-factor.md).

The [coefficient of determination](../../../../../coefficient-of-determination.md) is $R^2=1-\operatorname{RSS}/\operatorname{TSS}=0.7743$. The omnibus [F-test](../../../../../f-test.md) compares all 15 nonintercept coefficients with zero:

$$
F=\frac{(\operatorname{TSS}-\operatorname{RSS})/15}{\operatorname{RSS}/36}=8.2316,
$$

with reference $F_{15,36}$ and $p=1.2544\times10^{-7}$. This says at least one [factor](../../../../../regression-factor.md) contrast is nonzero under the assumed error model. There is one observation per cell, so an unrestricted goods-country [interaction](../../../../../interaction-statistics.md) would saturate the model, leaving zero [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md). Without replication or a specified [interaction](../../../../../interaction-statistics.md) structure, the residual variation cannot be separated into [interaction](../../../../../interaction-statistics.md) and independent error.

The second fit applies a [logarithmic transformation](../../../../../logarithmic-transformation.md) and fits the same [factor](../../../../../regression-factor.md) design to $Z_{gc}=\log Y_{gc}$. The [Gaussian log-response model](../../../../../gaussian-log-response-model.md) is

$$
\log Y_{gc}=\mu+a_g+b_c+\varepsilon_{gc}.
$$

Its intercept exponentiates to a fitted Software–UK conditional [median](../../../../../median.md) of $e^{4.5267}\approx92.45$ million euros. Goods coefficients now give multiplicative ratios to Software, and country coefficients give multiplicative ratios to the UK. The estimated country ratios are

$$
\boxed{\mathrm{France/UK}=e^{-1.6800}=0.1864,\quad
\mathrm{Germany/UK}=e^{-0.2447}=0.7830,\quad
\mathrm{rest/UK}=e^{-0.5033}=0.6045.}
$$

For example the Books ratio is $e^{1.6415}\approx5.16$ and the Sports Equipment ratio is $e^{-1.8364}\approx0.1594$, consistently across countries. The model assumes common relative, rather than common absolute, country effects. It also guarantees positive retransformed fitted values. Under normal log errors, the original-scale conditional mean is $e^{\eta+\sigma^2/2}$, whereas $e^\eta$ is the conditional [median](../../../../../median.md) and [geometric mean](../../../../../geometric-mean.md). Correcting the [retransformation bias](../../../../../retransformation-bias.md) here multiplies the naive predictions by approximately $e^{0.127406/2}=1.0658$.

The log-scale [residual standard error](../../../../../residual-standard-error.md) is $0.3569$, with the same 36 [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md), corresponding to a typical multiplicative error multiplier $e^{0.3569}\approx1.429$. France and the rest remain significant reference-country contrasts; Germany remains nonsignificant at 5%. The log-scale significant reference-goods contrasts are Books, Music, Videos/DVDs, Clothing, Sports Equipment, Electronic Goods, Groceries and Leisure Travel. Event Tickets, Toys, Video Games and Housewares do not individually differ significantly from Software at that level. These [p-values](../../../../../p-value.md) remain subject to the usual [multiple testing](../../../../../multiple-hypothesis-testing.md) qualification.

The log-scale $R^2=0.9381$ is computed using variation in the logarithms, so it cannot by itself establish better fit on the original response scale. The change is plausible because spending varies widely in magnitude and relative discrepancies are more meaningful than constant absolute discrepancies, but it should be assessed with [regression diagnostics](../../../../../regression-diagnostics.md), especially a [residual-versus-fitted plot](../../../../../residual-versus-fitted-plot.md) and a [normal Q-Q plot](../../../../../normal-q-q-plot.md). The minimum residual near $-1.01$ merits inspection; the command summaries alone do not verify independent normal errors. Moreover these responses are forecasts, so the inferential [p-values](../../../../../p-value.md) have a literal sampling interpretation only if an appropriate stochastic model for their uncertainty is justified.

The log-scale [analysis of variance](../../../../../analysis-of-variance.md) adds Goods and then Country. In this balanced design their effect spaces are orthogonal after removing the intercept, so the [sequential sums of squares](../../../../../sequential-sum-of-squares.md) equal the corresponding adjusted [factor](../../../../../regression-factor.md) sums and are unchanged by reversing the two [factors](../../../../../regression-factor.md):

$$
SS_G=4\sum_g(\overline Z_{g\cdot}-\overline Z_{\cdot\cdot})^2=47.85186,\qquad
SS_C=13\sum_c(\overline Z_{\cdot c}-\overline Z_{\cdot\cdot})^2=21.60350.
$$

The [residual sum of squares](../../../../../residual-sum-of-squares.md) is $4.58662$, giving $MS_E=4.58662/36=0.127406$. Thus

$$
\boxed{F_G=\frac{47.85186/12}{0.127406}=31.29875\quad(12,36\text{ df}),\qquad
F_C=\frac{21.60350/3}{0.127406}=56.52133\quad(3,36\text{ df}).}
$$

Their tiny upper-tail [p-values](../../../../../p-value.md) show strong overall goods and country effects under the log-error model; a globally significant country [factor](../../../../../regression-factor.md) is compatible with the nonsignificant individual Germany contrast. The omnibus fit statistic is $36.3433$ on $(15,36)$ degrees of freedom, whose [p-value](../../../../../p-value.md) is approximately $3.14\times10^{-17}$. The printed zero reflects numerical formatting, not an exactly zero [probability](../../../../../probability.md).

If two cell entries were missing, retain their correct [factor](../../../../../regression-factor.md) labels and mark those responses unavailable, rather than shifting the remaining scan values into different cells. Fit the additive models to the 50 observed cells, assuming the missingness mechanism permits those observations to be analyzed without selection bias. All [factor](../../../../../regression-factor.md) levels remain represented, and the row-column incidence graph remains connected: any two goods rows still share an observed country, since only two edges of the complete layout have been removed, and every country still has many observed goods. By [identifiability of an incomplete two-factor additive design](../../../../../identifiability-of-an-incomplete-two-factor-additive-design.md), the design therefore still has rank $13+4-1=16$. Hence

$$
\boxed{\text{two missing cells leave }50-16=34\text{ residual degrees of freedom}.}
$$

The coefficients and their [covariance](../../../../../covariance.md) must be recomputed by the observed-cell [ordinary least squares](../../../../../ordinary-least-squares.md) equations. The balanced row-mean-plus-column-mean formulas and common within-factor [standard errors](../../../../../standard-error.md) no longer apply. Goods and Country effects are generally no longer orthogonal, so sequential ANOVA sums can depend on order; [factor](../../../../../regression-factor.md) tests adjusted for the other [factor](../../../../../regression-factor.md) should use nested model comparisons. Missing cells do not restore replication or make an unrestricted [interaction](../../../../../interaction-statistics.md) test possible: that larger model still fits every observed cell exactly. If missingness depends on the unavailable spending values, additional modelling of that mechanism would be needed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

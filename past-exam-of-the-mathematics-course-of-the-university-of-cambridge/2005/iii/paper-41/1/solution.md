<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

`scan` reads the numerical prices, including the three missing-value markers, into a vector. The data must be read row by row for the subsequent factor construction to match them. The [sample size](../../../../../sample-size.md) available for analysis is therefore $37$, rather than $40$. The numerical summary describes the observed prices: the [sample median](../../../../../sample-median.md) is £43.54 and the [sample mean](../../../../../sample-mean.md) is £46.94. The upper tail, particularly the boots, raises the [sample mean](../../../../../sample-mean.md) above the [sample median](../../../../../sample-median.md). These summaries mix very different products and are not adjusted country comparisons.

The two character scans create labels. `gl(8,5,length=40,labels=item)` makes a [regression factor](../../../../../regression-factor.md) with each of eight item labels repeated five times. `gl(5,1,length=40,labels=country)` cycles through the five country labels once for each item. For a [regression factor](../../../../../regression-factor.md) and numerical response, the two `plot` commands produce grouped [box plots](../../../../../box-plot.md). The country [box plots](../../../../../box-plot.md) suggest lower US prices, while the item [box plots](../../../../../box-plot.md) show particularly expensive boots and inexpensive cardigans. They are descriptive displays of this small basket, with different item compositions where prices are missing; they cannot separate country effects from item effects.

The first `lm` fits an additive [two-way analysis of variance](../../../../../two-way-analysis-of-variance.md):

$$
p_{ij}=a+c_j+d_i+\varepsilon_{ij},\qquad c_{\mathrm{UK}}=0,\quad d_{\mathrm{jeans}}=0.
$$

The constraints are R's usual [treatment coding](../../../../../treatment-coding.md). The [normal linear model](../../../../../normal-linear-model.md) used for the printed tests assumes [independent](../../../../../independent-random-variables.md) errors with common [variance](../../../../../variance-split.md) and approximately a [normal distribution](../../../../../normal-distribution.md), and no item-by-country [interaction](../../../../../interaction-statistics.md) in the mean. Missing prices are omitted, leaving $37$ responses and $1+4+7=12$ independent mean coefficients. Thus the [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md) are $37-12=25$. This deletion is defensible for the conditional price model when missingness does not depend on the unobserved error after conditioning on the two factors; the output itself does not establish such a [missing-data mechanism](../../../../../missing-data-mechanism.md).

The `anova` tables report [sequential sums of squares](../../../../../sequential-sum-of-squares.md), rather than order-independent adjusted effects. If $R_0,R_C,R_I,R_{CI}$ are the [residual sums of squares](../../../../../residual-sum-of-squares.md) from the intercept-only, country-only, item-only and additive fits, the first order allocates $R_0-R_C$ to country and $R_C-R_{CI}$ to item. The second order allocates $R_0-R_I$ to item and $R_I-R_{CI}$ to country. Both allocations sum to the same total explained sum of squares, and both end with the same [residual sum of squares](../../../../../residual-sum-of-squares.md) $659.4$. The three missing combinations destroy [balanced factorial orthogonality](../../../../../balanced-factorial-orthogonality.md), so the allocation changes with order. To test country after allowing for items, use the country row in the second table; to test item after allowing for countries, use the item row in the first table. The first-entered rows do not supply those adjusted tests.

Each [mean square in ANOVA](../../../../../mean-square-in-anova.md) divides its [sum of squares in ANOVA](../../../../../sum-of-squares-in-anova.md) by its [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), and each printed [F-statistic](../../../../../f-statistic.md) divides that [mean square in ANOVA](../../../../../mean-square-in-anova.md) by $659.4/25=26.38$. In particular, the adjusted country [partial F-test](../../../../../partial-f-test-for-nested-linear-models.md) has

$$
F=\frac{1616.7/4}{659.4/25}=15.32,
$$

with an $F_{4,25}$ reference [F-distribution](../../../../../f-distribution.md) and [p-value](../../../../../p-value.md) approximately $1.86\times10^{-6}$. The adjusted item [partial F-test](../../../../../partial-f-test-for-nested-linear-models.md) gives $F=91.58$ on $7,25$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). Both factors contribute strongly under the additive [normal linear model](../../../../../normal-linear-model.md). The larger item [sum of squares in ANOVA](../../../../../sum-of-squares-in-anova.md) measures the much greater differences between these products, but is not evidence that every pair of items differs significantly.

The intercept $50.799$ is the fitted UK price for the reference jeans, not their observed price and not the overall [sample mean](../../../../../sample-mean.md). Each country [regression coefficient](../../../../../regression-coefficient.md) is its adjusted price difference from the UK, assumed common across items: Sweden is £5.224 lower, France £10.708 lower, Germany £7.676 lower and the US £21.328 lower. Each item [regression coefficient](../../../../../regression-coefficient.md) is its adjusted difference from the reference jeans, assumed common across countries. Thus the fitted UK boots price is $50.799+52.854=103.653$, and the fitted US boots price is $103.653-21.328=82.325$.

The coefficient [standard errors](../../../../../standard-error.md) come from $s^2(X^TX)^{-1}$, where $s^2=659.4/25$ and $X$ is the [design matrix](../../../../../design-matrix.md). Dividing each estimate by its [standard error](../../../../../standard-error.md) gives the displayed [Student t-test](../../../../../student-s-t-test.md) statistic, with $25$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The stars summarize the corresponding two-sided [p-values](../../../../../p-value.md). The individual tests compare each indicated country or item with its reference level, conditional on all other additive terms; they are neither tests of every pairwise comparison nor a simultaneous [confidence interval](../../../../../confidence-interval.md) procedure. In particular, Sweden's [p-value](../../../../../p-value.md) $0.0626$ provides weaker evidence than the other country contrasts, and does not establish equality with the UK. The intercept test has little substantive relevance, and interpreting many individual stars also raises [multiple hypothesis testing](../../../../../multiple-hypothesis-testing.md) issues.

The [residual standard error](../../../../../residual-standard-error.md) $s=5.136$ measures unexplained prices in pounds. With total corrected sum of squares $T$, the [coefficient of determination](../../../../../coefficient-of-determination.md) and [adjusted coefficient of determination](../../../../../adjusted-coefficient-of-determination.md) are

$$
R^2=1-\frac{659.4}{T}=0.9647,\qquad
\overline R^2=1-\frac{659.4/25}{T/36}=0.9492.
$$

Much of this impressive fit is due to the large differences between items. The overall [F-test](../../../../../f-test.md) compares the additive fit with a constant mean: $F=((T-659.4)/11)/(659.4/25)=62.12$ on $11,25$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). It tests that all eleven non-intercept coefficients vanish, not that the additive model is adequate. [Regression diagnostics](../../../../../regression-diagnostics.md) should examine [regression residuals](../../../../../regression-residual.md), changing price variability across items and possible [interaction](../../../../../interaction-statistics.md). Percentage differences may be more plausible than common pound differences, motivating a [natural logarithm](../../../../../natural-logarithm.md) of price. No random sample of countries or products, and no independent replication of a price within a cell, is supplied; broad claims about all designer goods or the causes of country differences require more than these conditional tests.

Finally, `Item*Country` expands to both main effects and their full [interaction](../../../../../interaction-statistics.md). A cell-means parameterization has one separate fitted mean for every observed cell. With one response per cell its [design matrix](../../../../../design-matrix.md) has row [matrix rank](../../../../../matrix-rank.md) $37$, while the full $8\times5$ layout nominally has $40$ coefficients. Three coefficient combinations are aliased because their cells are missing. This is [saturation of an unreplicated two-factor regression](../../../../../saturation-of-an-unreplicated-two-factor-regression.md): every observed price is fitted exactly and the [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md) are zero. **The final fit has zero residuals, $R^2=1$ and no residual-based estimate of the error variance or ordinary interaction significance test.** The printed numerical summary will mark three coefficients unestimable; coefficient [standard errors](../../../../../standard-error.md), tests and adjusted $R^2$ involve undefined division by zero, potentially appearing as `NaN` or `Inf` according to numerical roundoff. Perfect interpolation here is a consequence of a [saturated statistical model](../../../../../saturated-statistical-model.md), not evidence for a superior predictive model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

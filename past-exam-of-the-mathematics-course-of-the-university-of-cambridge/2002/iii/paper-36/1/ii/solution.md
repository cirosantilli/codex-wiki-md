<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Both fits are the same additive [two-way analysis of variance](../../../../../../two-way-analysis-of-variance.md) model: a common intercept, five country effects represented by four contrasts, and eight item effects represented by seven contrasts. The three missing cells are omitted, leaving $37$ observations and model rank $1+4+7=12$, hence $25$ residual degrees of freedom. The [residual sum of squares](../../../../../../residual-sum-of-squares.md) is $659.44$ in either ordering, giving

$$
\boxed{\widehat\sigma^2=659.44/25=26.3776,\qquad\widehat\sigma\simeq5.136\text{ pounds}}.
$$

These are [sequential sums of squares](../../../../../../sequential-sum-of-squares.md), so each row measures the improvement when that factor is added after the preceding factors. The country-first sum $1115.56$ describes its unadjusted contribution before accounting for item; its displayed $F=10.573$ and $p=3.73\times10^{-5}$ are not the country-adjusted-for-item test. When country is added after item, its extra sum is $1616.74$, giving

$$
\boxed{F_{\text{country}\mid\text{item}}
=\frac{1616.74/4}{659.44/25}=15.323,\qquad p\simeq1.86\times10^{-6}}.
$$

Thus the additive [normal linear model](../../../../../../normal-linear-model.md) gives strong evidence of country differences after accounting for the different products. Conversely, item added after country has extra sum $16910.20$, so

$$
\boxed{F_{\text{item}\mid\text{country}}
=\frac{16910.20/7}{659.44/25}=91.583,\qquad p\simeq3.19\times10^{-16}}.
$$

The printed zero for this [probability](../../../../../../probability.md) is numerical formatting, not a [probability](../../../../../../probability.md) literally equal to zero. Product differences are much larger than residual variation, as expected from their different scales.

The explanation for the order dependence is that [missing cells can destroy factor orthogonality in two-way ANOVA](../../../../../../missing-cells-can-destroy-factor-orthogonality-in-two-way-anova.md). A complete equally replicated crossed design would make centered country and item indicator columns orthogonal. Here the missing observations change the item mix across countries and the country mix across items, so the two factor subspaces are not orthogonal. The two sequential partitions still have the same total explained sum: $1115.56+16910.20=16409.02+1616.74=18025.76$ to the displayed precision. For inference about either factor conditional on the other, compare the full model with the reduced model that omits that factor, rather than interpreting its first-entry sum as adjusted evidence.

The omnibus country test does not identify the particular country contrasts. As an extension, fitting the supplied price table gives the item-adjusted UK-minus-US contrast about $21.33$ pounds, with [standard error](../../../../../../standard-error.md) $2.824$ and an ordinary Gaussian-model $95\%$ [confidence interval](../../../../../../confidence-interval.md) approximately $[15.51,27.14]$ pounds. This is a derived model contrast, with [Student t-distribution](../../../../../../student-s-t-distribution.md) reference on $25$ degrees of freedom; simultaneous exploration of many country pairs requires control for [multiple hypothesis testing](../../../../../../multiple-hypothesis-testing.md).

Check residuals against fitted values, product and country, together with a normal [Q-Q plot](../../../../../../q-q-plot.md) and influential observations. The [homoscedasticity](../../../../../../homoscedasticity.md) assumption on absolute prices may be doubtful because expensive products can have larger absolute variation. A model for logarithmic prices gives multiplicative country effects and can make the scale assumption more plausible. Country-by-item [interaction terms](../../../../../../interaction-term.md) would allow discounts to differ by product, but there is at most one observed value per cell: an unrestricted interaction saturates the $37$ observed means and leaves no pure-error degrees of freedom, so it cannot be tested against [independent](../../../../../../independent-random-variables.md) measurement noise from these data alone. Additional products or genuine cell replication would support that extension. The selected products and non-random missing entries also limit claims about a whole country's consumer prices; the conditional inference is for the stated additive model and observed price collection.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

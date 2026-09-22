<h1 id="13i/solution">Solution</h1>

↑ **Parent:** [13I](../13i.md)

The data are read row by row into a [vector](../../../../../vector.md) of 84 prices. The first factor cycles through the six goods within each row; the second repeats each of the fourteen resort levels for six entries. Thus the [linear regression](../../../../../linear-regression-split.md) fits one observation per resort-good cell, after taking natural logarithms. With treatment coding, its underlying statistical model is

$$
\log P_{ij}=\alpha+r_i+g_j+\varepsilon_{ij},\qquad r_1=g_1=0,\qquad\varepsilon_{ij}\ \text{independent }N(0,\sigma^2),
$$

for resorts $i=1,\ldots,14$ and goods $j=1,\ldots,6$. This is an additive [two-way analysis of variance](../../../../../two-way-analysis-of-variance.md) on log prices, equivalently a multiplicative resort/goods model on the price scale, with no interaction. There are $1+13+5=19$ fitted parameters and $84-19=\boxed{65\text{ residual degrees of freedom}}$.

In a balanced complete table, the fitted log price is the resort row mean plus the goods column mean minus the grand mean. Thus every resort coefficient is its row mean minus the Algarve row mean, and every goods coefficient is its column mean minus the meal column mean. The intercept is the fitted mean log price for a meal in Algarve, not necessarily the observed log price in that cell. Exponentiating coefficients gives price multipliers: the beer coefficient corresponds to approximately $e^{-2.1084}=0.1214$ times the meal scale, and car hire to $e^{2.8016}=16.47$ times that scale. Likewise the Sorrento resort effect gives a common factor $e^{0.5981}=1.819$ relative to Algarve, if the no-interaction model is valid.

The standard errors are computed from $s^2(X^TX)^{-1}$ with $s=0.3425$. Balance gives goods-contrast standard error $s\sqrt{2/14}=0.1295$ and resort-contrast standard error $s\sqrt{2/6}=0.1978$. Each reported t statistic is its estimated coefficient divided by its standard error. Under the Gaussian model and the corresponding zero-coefficient null, it has a [Student t-distribution](../../../../../student-s-t-distribution.md) with 65 degrees of freedom; the reported [probabilities](../../../../../probability.md) are two-sided tail [probabilities](../../../../../probability.md). All goods contrasts are strongly significant, largely reflecting unlike goods and units of purchase. Among the resort contrasts, Costa del Sol, Majorca, Florida, Sorrento, Sicily and Madeira have unadjusted [probabilities](../../../../../probability.md) below $0.05$. This is six separate comparisons with Algarve, not a simultaneous ranking guarantee or an omnibus test of all resorts. Multiple comparisons and model adequacy must be considered before declaring a universal cheapest resort.

The residual standard error measures variation on the log scale; $e^{0.3425}\simeq1.408$ is a typical multiplicative one-standard-deviation factor. Under the [lognormal distribution](../../../../../log-normal-distribution.md), $\exp(\widehat\alpha+\widehat r_i+\widehat g_j)$ estimates the conditional median/geometric mean price, while the arithmetic mean has the additional factor $\exp(\sigma^2/2)$. The reported $R^2=0.962$ means **96.2 percent of the observed log-price sum of squares around its overall mean is explained**. It does not mean resorts alone explain that fraction, nor that 96.2 percent of variation on the original price scale is explained.

With only one observation per cell, unrestricted goods-by-resort interactions cannot be estimated separately from residual error. The model assumes comparable quoted items, approximately common log-error [variance](../../../../../variance-split.md), independent errors and common resort multipliers across goods. Residuals can reveal failures, such as a particular resort having unusually costly taxis but ordinary prices for other goods. The intercept's test against zero concerns a fitted baseline geometric price of one pound; it is not an assessment of the overall model's validity.

## ↑ Ancestors (10)

1. [13I](../13i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

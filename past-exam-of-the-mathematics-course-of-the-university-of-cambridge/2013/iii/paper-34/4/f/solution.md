<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Integrate each supplied predictive density to get its [cumulative distribution function](../../../../../../cumulative-distribution-function.md) $F_t$, then form the [sequential probability integral transform](../../../../../../sequential-probability-integral-transform.md)

$$
\boxed{U_t=F_t(y_t).}
$$

For a correct continuous one-step conditional predictive model, $\mathbb P(U_t\le u\mid y_1,\ldots,y_{t-1})=u$. Iterating this identity shows that the $U_t$ are independent uniform variables. A histogram or quantile plot checks uniformity; serial plots and autocorrelations check for temporal structure left unexplained by the forecasts.

Also inspect empirical coverage of central [prediction intervals](../../../../../../prediction-interval.md), tail exceedances and interval widths, assessing calibration together with sharpness. These checks need only the supplied forecasts and observations. Compare chosen [predictive discrepancy statistics](../../../../../../predictive-discrepancy-statistic.md) with simulated uniform reference sequences. A total log score alone is a relative reward and does not provide a universal absolute goodness-of-fit threshold.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

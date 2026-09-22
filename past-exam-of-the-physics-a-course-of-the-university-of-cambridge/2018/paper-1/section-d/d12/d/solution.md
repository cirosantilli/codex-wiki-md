<h1 id="section-d/d12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a candidate attenuation coefficient, the one-second expected count is $\mu_n=2018.5e^{-bn}$. The model predictions are

$$
\begin{array}{c|rrrrrrrr}
n&1&2&3&4&5&6&7&8\\ \hline
b=1&742.56&273.17&100.50&36.97&13.60&5.00&1.84&0.677\\
b=1.1&671.90&223.66&74.45&24.78&8.25&2.75&0.914&0.304
\end{array}
$$

Use first the conservative signal-dominated range $n=1,\ldots,4$, where the count approximation is reliable and background is a small correction. Using the estimated errors from part (c), the weighted residual statistic is

$$
Q_{\mathrm{obs}}(b)=\sum_{n=1}^4\frac{(y_n-\mu_n)^2}{y_n}.
$$

It gives $\boxed{Q_{\mathrm{obs}}(1)=4.45,\qquad Q_{\mathrm{obs}}(1.1)=12.74}$. Since both $b$ candidates are fixed and $N_0$ was calibrated independently, neither was fitted to these four counts: the approximate reference has $\nu=4$, not three. The upper-tail probabilities are approximately $0.349$ and $0.0126$, respectively. Thus $b=1$ is compatible with the scatter, whereas $b=1.1$ is disfavored at the usual $5\%$ level in this approximate test.

A [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md), using model variances instead of estimated observed variances, gives the same preference:

$$
Q_{\mathrm P}(1)=4.04,\quad Q_{\mathrm P}(1.1)=15.62,\qquad p\simeq0.401,\ 0.00357.
$$

Including the fifth point also leaves the decision unchanged: the estimated-error statistics are $8.37$ and $12.74$ on five degrees of freedom, with approximate upper-tail probabilities $0.137$ and $0.0259$; the Pearson statistics are $6.34$ and $15.63$. Hence

$$
\boxed{b=1\text{ provides the better exponential fit}.}
$$

The small uncertainty in $N_0$ contributes correlated prediction uncertainty, as in [chi-squared comparison of a calibrated attenuation model](../../../../../../chi-squared-comparison-of-a-calibrated-attenuation-model.md), but is negligible compared with the one-second counting errors here. Choosing the test range after inspecting the observations limits a strict interpretation of its nominal significance; the numerical comparison and its stated range are the relevant evidence.

If all eight observations are inserted into the estimated-error formula, the totals are $14.99$ and $22.48$. Their nominal eight-degree-of-freedom calibration is unreliable because the final expected counts are much smaller than one for some predictions. In fact the full-range Pearson statistics are $43.34$ and $118.25$, exposing the late excess much more strongly. The full [Poisson deviance](../../../../../../poisson-deviance.md) values are $24.09$ and $47.03$, again favoring $b=1$ but signaling that a background-free exponential is inadequate over the complete range. These sparse-count comparisons should not be used to claim that either unmodified model explains all eight measurements.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

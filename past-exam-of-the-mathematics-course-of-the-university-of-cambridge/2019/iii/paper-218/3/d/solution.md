<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The usual residual-deviance chi-squared calibration is unreliable because random effects are estimated and integrated out, changing both the effective degrees of freedom and the null distribution. Use a [parametric bootstrap](../../../../../../parametric-bootstrap.md): fit the reported GLMM; compute an observed dispersion statistic such as the Pearson statistic or its ratio to nominal residual degrees of freedom; for each bootstrap replicate draw ten player effects from $N(0,0.1168)$, simulate all 60 Poisson responses from the fitted conditional means, refit the same GLMM, and recompute the statistic. With $B$ replicates, estimate the upper-tail p-value by

$$
\widehat p=\frac{1+\#\{T_b\geq T_{\mathrm{obs}}\}}{B+1}.
$$

Reject at $5\%$ when $\widehat p<0.05$, equivalently when $T_{\mathrm{obs}}$ exceeds the empirical $95$th percentile of the bootstrap null distribution.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fit a trend $\widehat T_t$, form $D_t=X_t-\widehat T_t$, and estimate the period-25 seasonal effect by

$$
\widehat S_j=\frac1M\sum_{r=0}^{M-1}D_{j+25r},
\qquad j=1,\ldots,25.
$$

The residual is $R_t=X_t-\widehat T_t-\widehat S_{t\bmod25}$. This additive decomposition is sensible when seasonal amplitude does not systematically change with the level or trend; multiplicative seasonality would require a logarithmic transform or ratio decomposition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

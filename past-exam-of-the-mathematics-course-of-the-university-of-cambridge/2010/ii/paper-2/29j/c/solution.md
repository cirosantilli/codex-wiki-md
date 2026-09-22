<h1 id="29j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\sigma^2=\Sigma_\eta>0$ and assume $V_0>0$. The scalar [Kalman filter](../../../../../../kalman-filter.md) reduces to

$$
V_{t+1}=\frac{V_t\sigma^2}{V_t+\sigma^2},\qquad
\hat X_{t+1}=\frac{\sigma^2\hat X_t+V_tY_{t+1}}{V_t+\sigma^2}.
$$

Taking reciprocal variance and dividing the mean by variance gives

$$
V_{t+1}^{-1}=V_t^{-1}+\sigma^{-2},\qquad
\hat X_{t+1}/V_{t+1}=\hat X_t/V_t+Y_{t+1}/\sigma^2.
$$

Thus

$$
\hat X_t=\frac{\sigma^2\hat X_0/V_0+\sum_{j=1}^tY_j}{\sigma^2/V_0+t}.
$$

Since the process noise is zero and $A=1$, $X_t=X_0$ and $Y_j=X_0+\eta_j$. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $t^{-1}\sum_jY_j\to X_0$ almost surely. The prior's finite weight vanishes in the displayed formula, so **both limits equal $X_0$ almost surely.** A zero prior variance instead means $X_0$ is known, and the assertion follows directly without reciprocal-variance formulas.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29J](../../29j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

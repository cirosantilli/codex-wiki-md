<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [martingale residual](../../../../../../martingale-residual.md) is observed minus model-expected event count:

$$
\widehat M_i=v_i-\widehat\Lambda_i(x_i),
$$

where $\widehat\Lambda_i$ is the fitted individual [cumulative hazard](../../../../../../cumulative-hazard-function.md). Under an adequate model it estimates the terminal value of a counting-process [martingale](../../../../../../martingale-split.md).

Fit a model omitting the continuous explanatory variable $z$, plot $\widehat M_i$ against $z_i$, and add a flexible smooth curve. A curve fluctuating around zero without structure supports omission. A monotone or curved trend indicates that event incidence still depends on $z$, suggesting inclusion of $z$ or a nonlinear transformation of it. The residuals are highly skewed, so the smoothed trend is more informative than an assumption of Gaussian scatter.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

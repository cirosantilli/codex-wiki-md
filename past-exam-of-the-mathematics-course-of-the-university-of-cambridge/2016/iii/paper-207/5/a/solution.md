<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The transformed event time is unit exponential, and the transformed censoring time remains a censoring time because $H$ is increasing. Under [independent censoring](../../../../../../independent-censoring.md) and a correctly fitted model, the [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) of the [survivor function](../../../../../../survival-function.md) for the [Cox–Snell residuals](../../../../../../cox-snell-residual.md) $\widehat H(x_i)$ should approximate $e^{-u}$.

Thus **a logarithmic survivor plot should follow a straight line through the origin with slope minus one**:

$$
\boxed{\log\widehat F_{\mathrm{res}}(u)\approx-u.}
$$

The empirical plot is a step function around that line. Systematic curvature suggests model misspecification; the late part is less stable when the [risk set](../../../../../../risk-set.md) is small. The retained event indicators $v_i$ must be used rather than treating censored residuals as complete event times.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

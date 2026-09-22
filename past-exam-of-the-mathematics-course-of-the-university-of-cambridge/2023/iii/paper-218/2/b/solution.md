<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At lag $h$, the plot shows the [sample autocorrelation function](../../../../../../sample-autocorrelation-function.md)

$$
\widehat\rho(h)=
\frac{\sum_{t=h+1}^n(X_t-\overline X)(X_{t-h}-\overline X)}
{\sum_{t=1}^n(X_t-\overline X)^2}.
$$

Under a [white noise process](../../../../../../white-noise.md), each fixed nonzero-lag sample autocorrelation is approximately $N(0,1/n)$, so the dashed pointwise $95\%$ reference lines are approximately $\pm1.96/\sqrt n$.

The first nonzero-lag bar is well above the upper line, which contradicts the zero autocorrelation expected from white noise. Since the plot then largely cuts off, an [moving-average process of order one](../../../../../../moving-average-process-of-order-one.md) is a plausible model; with the sampling interval as the time unit this is an $\operatorname{ARMA}(0,1)$ model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

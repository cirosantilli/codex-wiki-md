<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The useful [autoregressive model](../../../../../../autoregressive-model.md) is for the squares, not for signed observations. Put $Y_t=X_t^2$ and

$$
u_t=(\varepsilon_t^2-1)(\alpha_0+\alpha_2Y_{t-2}).
$$

Then

$$
\boxed{Y_t=\alpha_0+\alpha_2Y_{t-2}+u_t.}
$$

The errors form a [martingale difference sequence](../../../../../../martingale-difference-sequence.md) relative to the noise history, because the current standardized noise is independent of the past. When the [fourth moment](../../../../../../fourth-moment.md) is finite they have finite [variance](../../../../../../variance-split.md) and are uncorrelated across distinct times, although their [conditional variance](../../../../../../conditional-variance.md) depends on the regressor. In centered form, $Y_t-m_2=\alpha_2(Y_{t-2}-m_2)+u_t$.

For [ordinary least squares](../../../../../../ordinary-least-squares.md), use the $n-2$ response-regressor pairs $y_t=X_t^2$, $r_t=X_{t-2}^2$, $t=3,\ldots,n$. With their separate means $\bar y$ and $\bar r$, minimize $\sum_{t=3}^n(y_t-a-br_t)^2$. If the regressor sum of squares is positive, the estimators are

$$
\boxed{\widehat\alpha_2=\frac{\sum_{t=3}^n(r_t-\bar r)(y_t-\bar y)}{\sum_{t=3}^n(r_t-\bar r)^2},\qquad
\widehat\alpha_0=\bar y-\widehat\alpha_2\bar r.}
$$

The two means use the matched pairs; replacing them indiscriminately by a single full-sample mean is not the exact least-squares formula. The noise-series representation supplies an [ergodic stationary process](../../../../../../ergodic-stationary-process.md). If $3\alpha_2^2<1$, finite regressor [second moments](../../../../../../second-moment.md) and the error's zero [conditional expectation](../../../../../../conditional-expectation.md) justify the usual population regression and [statistical consistency](../../../../../../consistency-statistics.md) argument. The observations still define a finite-sample least-squares fit outside that moment range, but the ordinary finite-[variance](../../../../../../variance-split.md) justification must not be claimed there. If parameter constraints are required, minimize the same criterion subject to $a>0$ and $0<b<1$, rather than assert that unconstrained estimates automatically satisfy them.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

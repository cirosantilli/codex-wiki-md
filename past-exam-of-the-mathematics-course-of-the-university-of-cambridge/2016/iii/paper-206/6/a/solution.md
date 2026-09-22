<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $t_{ij}$ for stirring rate of observation $i$ in furnace $j$. The [independent random-intercept and random-slope model](../../../../../../independent-random-intercept-and-random-slope-model.md) is

$$
Y_{ij}=\beta_0+\beta_1t_{ij}+u_j+v_jt_{ij}+\varepsilon_{ij},
\qquad
\begin{pmatrix}u_j\\v_j\end{pmatrix}\overset{\mathrm{iid}}\sim
N_2\!\left(0,\begin{pmatrix}\tau_0^2&0\\0&\tau_1^2\end{pmatrix}\right),
\qquad\varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Errors and [random effects](../../../../../../random-effect.md) are independent. The separate R terms `(1 | furnace)` and `(0 + stir | furnace)` impose independent [random intercepts](../../../../../../random-intercept.md) and [random slopes](../../../../../../random-slope.md); `(1 + stir | furnace)` would instead estimate their covariance as well. The estimates are

$$
\boxed{\widehat\beta_0=277.6636,\quad\widehat\beta_1=0.5601,\quad
\widehat\tau_0^2=48.73800,\quad\widehat\tau_1^2=0.01316,\quad
\widehat\sigma^2=36.29950.}
$$

The corresponding estimated standard deviations are $6.9813$, $0.1147$, and $6.0249$; they are not additional parameters.

For a furnace with predictor vector $t_j$, the marginal formulation, obtained by integrating the Gaussian [random effects](../../../../../../random-effect.md), is

$$
Y_j\sim N\!\left(\beta_0\mathbf1+\beta_1t_j,
\tau_0^2\mathbf1\mathbf1^T+\tau_1^2t_jt_j^T+\sigma^2I\right),
$$

independently across furnaces. In particular,

$$
\operatorname{Cov}(Y_{ij},Y_{kj})=\tau_0^2+\tau_1^2t_{ij}t_{kj}+\sigma^2\mathbf1_{\{i=k\}}.
$$

In stacked notation $Y=X\beta+Zb+\varepsilon$, $b\sim N(0,D)$, giving the [Gaussian linear mixed model](../../../../../../gaussian-linear-mixed-model.md) marginal law $N(X\beta,V)$ with $V=ZDZ^T+\sigma^2I$.

The [residual-versus-fitted plot](../../../../../../residual-versus-fitted-plot.md) on page 17 has residuals of both signs over the fitted range, with no convincing smooth curvature or clear fan shape. Its [quantile-quantile plot](../../../../../../q-q-plot.md) is roughly straight in the central region, with some tail departures and a few large negative residuals. **There is no decisive visible violation**, but investigate those observations. These plots mainly address conditional observation errors; they do not validate the distribution of furnace [random effects](../../../../../../random-effect.md) or [independence](../../../../../../independent-random-variables.md) within furnaces. With only three furnaces, [normality](../../../../../../normal-distribution.md) and the [variance](../../../../../../variance-split.md) of the [random effects](../../../../../../random-effect.md) are especially difficult to assess.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

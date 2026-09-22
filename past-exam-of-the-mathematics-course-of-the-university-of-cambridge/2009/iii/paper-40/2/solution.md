<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [state-space model](../../../../../state-space-model-time-series.md) as printed supplies only uncorrelated [white noise](../../../../../white-noise.md). That is insufficient for the claimed normal [conditional distributions](../../../../../conditional-distribution.md). For example, take $S_0$ normal, [independent](../../../../../independent-random-variables.md) process noises $w_t$ taking values $\pm\sqrt W$ equally often, and [independent](../../../../../independent-random-variables.md) Gaussian observation noises. With $G=1$ and no previous observations, $S_1=S_0+w_1$ is a two-component shifted [mixture distribution](../../../../../mixture-distribution.md), not normal for $W>0$. Its characteristic function is $e^{i\mu s-P_0s^2/2}\cos(\sqrt W\,s)$, which has zeros, whereas a normal characteristic function has none. Similarly a non-Gaussian observation noise prevents the asserted conditional normal law for $X_t$.

The intended [scalar Gaussian Kalman recursion](../../../../../scalar-gaussian-kalman-recursion.md) requires $w_t\sim N(0,W)$ and $v_t\sim N(0,V)$ [independent](../../../../../independent-random-variables.md) of each other and of the previous state and observation history. Assume these Gaussian [independence](../../../../../independent-random-variables.md) conditions, $V>0$, $W\ge0$, and the given normal filtering law. Conditional on the past, $GS_{t-1}+w_t$ is a sum of [independent](../../../../../independent-random-variables.md) normals, hence

$$
\boxed{S_t\mid\mathcal F_{t-1}\sim N(m_t,R_t),\qquad m_t=G\widehat S_{t-1},\quad R_t=G^2P_{t-1}+W.}
$$

The new observation noise is [independent](../../../../../independent-random-variables.md) of $S_t$ and the past, so $X_t\mid S_t,\mathcal F_{t-1}\sim N(FS_t,V)$. Write $S_t=m_t+\eta_t$ and $X_t=Fm_t+F\eta_t+v_t$. The [independent](../../../../../independent-random-variables.md) normal pair $(\eta_t,v_t)$ shows directly that

$$
\binom{X_t}{S_t}\Bigm|\mathcal F_{t-1}\sim N\left(\binom{Fm_t}{m_t},\begin{pmatrix}Q_t&FR_t\\FR_t&R_t\end{pmatrix}\right),\qquad Q_t=F^2R_t+V.
$$

The [covariance](../../../../../covariance.md) $FR_t$ comes from the common $\eta_t$ term. Applying the [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) formula with $X_t$ as the conditioned coordinate gives the [Kalman filter](../../../../../kalman-filter.md) update

$$
\boxed{\widehat S_t=m_t+\frac{FR_t}{Q_t}(X_t-Fm_t),\qquad P_t=R_t-\frac{F^2R_t^2}{Q_t}=\frac{R_tV}{Q_t}.}
$$

The final expression verifies nonnegativity of the [posterior](../../../../../bayesian-posterior.md) [variance](../../../../../variance-split.md).

For $F=G=1$, define

$$
\boxed{\alpha_t=\frac{P_{t-1}+W}{P_{t-1}+W+V}.}
$$

The recursions become $\widehat S_t=(1-\alpha_t)\widehat S_{t-1}+\alpha_tX_t$ and $P_t=\alpha_tV$. If $P_t\to P$, then $\alpha_t\to\alpha=P/V$ and, with $c=W/V$,

$$
\alpha=\frac{\alpha+c}{\alpha+c+1}\quad\Longrightarrow\quad\alpha^2+c\alpha-c=0.
$$

The nonnegative solution is the [steady-state local-level Kalman gain](../../../../../steady-state-local-level-kalman-gain.md):

$$
\boxed{\alpha_\infty=\frac{\sqrt{c^2+4c}-c}{2},\qquad P=\frac{\sqrt{W^2+4WV}-W}{2}.}
$$

For $c=0$ the limit is zero; for $c>0$ it lies strictly between zero and one. These are exact conditional-law results under the additional Gaussian assumptions, not consequences of the weaker printed noise description alone.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

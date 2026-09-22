<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Interpret the forecasts as [best linear prediction from a finite past](../../../../../best-linear-prediction-from-a-finite-past.md). For a causal [autoregressive process](../../../../../autoregressive-model.md), the innovations are orthogonal to previous observations. If they also have zero conditional mean given the past, the same forecasts are conditional means; [white noise](../../../../../white-noise.md) by itself guarantees only the linear-prediction interpretation.

Let $m$ be the process mean and write its centered autoregression as $X_t-m=\sum_{j=1}^p\phi_j(X_{t-j}-m)+\epsilon_t$. Set $\widehat X_{T,h}=X_{T+h}$ for $h\le0$, and recursively put

$$
\boxed{\widehat X_{T,k}=m+\sum_{j=1}^p\phi_j(\widehat X_{T,k-j}-m),\qquad k\ge1.}
$$

The forecast is a linear combination of the observed last $p$ values. Subtracting the recursion from the future autoregression shows that the prediction error is a linear combination of future innovations, hence orthogonal to every observed value. This proves the optimal projection property, rather than merely suggesting that future noise should be replaced by zero. In particular,

$$
\widehat X_{T,1}=m+\sum_{j=1}^p\phi_j(X_{T+1-j}-m),\qquad
\widehat X_{T,2}=m+\phi_1(\widehat X_{T,1}-m)+\sum_{j=2}^p\phi_j(X_{T+2-j}-m).
$$

The empty sum for $p=1$ is zero. Taking $m=0$ gives the centered convention. This is the [recursive forecasts of an autoregressive process](../../../../../recursive-forecasts-of-an-autoregressive-process.md) construction.

For the stable order-one equation, use its stationary causal solution

$$
X_t=\sum_{j=0}^{\infty}\phi^j\epsilon_{t-j}.
$$

The series converges in mean square because $\sum\phi^{2j}<\infty$ and the [white noise](../../../../../white-noise.md) innovations have a common finite [variance](../../../../../variance-split.md) $\sigma^2$. Orthogonality of their distinct time indices gives

$$
\mathbb EX_t=0,\qquad
\operatorname{Cov}(X_{t+h},X_t)=\frac{\sigma^2\phi^{|h|}}{1-\phi^2}.
$$

Adding the deterministic mean therefore yields [weak stationarity](../../../../../weakly-stationary-process.md) for $Z$, with

$$
\boxed{\mathbb EZ_t=\mu,\quad \gamma_Z(h)=\frac{\sigma^2\phi^{|h|}}{1-\phi^2},\quad \rho_Z(h)=\phi^{|h|}.}
$$

The [autocorrelation function](../../../../../autocorrelation.md) assumes $\sigma^2>0$; a zero-variance process has no normalized correlation. A recursion from an arbitrary nonstationary initial value would have transient moments, so the stationary-solution interpretation is important here.

Iteration gives $X_{T+k}=\phi^kX_T+\sum_{j=1}^k\phi^{k-j}\epsilon_{T+j}$. The innovation sum is orthogonal to the observed past, giving

$$
\boxed{\widehat Z_{T,k}=\mu+\phi^k(Z_T-\mu)\longrightarrow\mu.}
$$

For the integrated process, the [backshift operator](../../../../../backshift-operator.md) subtracts consecutive levels, so $(I-B)W_t=\mu+(I-B)Y_t=\mu+X_t=Z_t$. Consequently $W_{T+k}=W_T+\sum_{j=1}^kZ_{T+j}$. If the last increment is observed, substitute its forecast and sum the [geometric progression](../../../../../geometric-progression.md):

$$
\boxed{\widehat W_{T,k}=W_T+k\mu+
\frac{\phi(1-\phi^k)}{1-\phi}(W_T-W_{T-1}-\mu).}
$$

This is the [forecasts of an integrated AR(1) process](../../../../../forecasts-of-an-integrated-ar-1-process.md) formula. Its final term is bounded as $k\to\infty$, even for negative $\phi$, hence **the forecast's long-run slope is the drift**:

$$
\boxed{\widehat W_{T,k}/k\longrightarrow\mu.}
$$

With an initial level orthogonal to future innovations, the level formula is also the best linear forecast from the observed levels. Without that initial-level condition, it is the increment-based recursive forecast, and the levels could contain additional predictive information. The level formula uses $T\ge2$, or a known $W_0$ when $T=1$. With just $W_1$ and no model for the initial level, the last increment cannot be recovered from the supplied observations; a one-observation level forecast would need that additional information.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

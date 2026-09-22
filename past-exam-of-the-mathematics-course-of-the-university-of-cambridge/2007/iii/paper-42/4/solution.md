<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the usual stochastic-integrability assumptions implicit in the price [stochastic differential equation](../../../../../stochastic-differential-equation.md): the coefficients have progressively measurable versions, the volatility is locally square integrable, and initial prices are finite deterministic positive numbers. A no-consumption [admissible trading strategy](../../../../../admissible-trading-strategy.md) consists of [predictable](../../../../../predictable-process.md) risky share holdings $\pi$ for which the price [stochastic integral](../../../../../stochastic-integral.md) exists and the [portfolio wealth](../../../../../portfolio-wealth.md) of the [self-financing portfolio](../../../../../self-financing-portfolio.md) is

$$
X_t=x+\int_0^t\pi_s^T\,dS_s.
$$

The remainder $X_t-\pi_t^TS_t$ is held in the unit cash asset. Admissibility requires $X_t\geq-a$ throughout the horizon for some deterministic finite $a$; the more restrictive nonnegative-wealth convention also works. A finite-horizon [arbitrage](../../../../../arbitrage.md) is such a strategy with $x=0$, $X_T\geq0$ almost surely and $P(X_T>0)>0$. The lower bound is essential to exclude doubling strategies.

Interpret the stated uniform ellipticity as $\sigma_t\sigma_t^T\geq\varepsilon I$ for a deterministic $\varepsilon>0$. If $|\mu_t|\leq K$, the [market price of risk](../../../../../market-price-of-risk.md) is bounded:

$$
\lambda_t=\sigma_t^{-1}\mu_t,\qquad |\lambda_t|^2=\mu_t^T(\sigma_t\sigma_t^T)^{-1}\mu_t\leq\frac{K^2}{\varepsilon}.
$$

The authoritative PDF puts both integrals inside the exponent. With that interpretation,

$$
Z_t=\exp\left(-\int_0^t\lambda_s^T\,dW_s-\frac12\int_0^t|\lambda_s|^2ds\right),\qquad dZ_t=-Z_t\lambda_t^T\,dW_t.
$$

On every finite horizon $T$, boundedness of $\lambda$ gives the [Novikov condition](../../../../../novikov-s-condition.md):

$$
\mathbb E\exp\left(\frac12\int_0^T|\lambda_s|^2ds\right)\leq\exp\left(\frac{K^2T}{2\varepsilon}\right)<\infty.
$$

Hence the positive [stochastic exponential](../../../../../doleans-dade-exponential.md) $Z$ is a true [martingale](../../../../../martingale-split.md) with $\mathbb EZ_T=1$. Define the equivalent probability measure $Q_T$ by $dQ_T=Z_T\,dP$. The [Girsanov theorem](../../../../../girsanov-theorem.md) says that $W_t^Q=W_t+\int_0^t\lambda_sds$ is a [Brownian motion](../../../../../brownian-motion-split.md) under $Q_T$, up to time $T$. Consequently

$$
dS_t=\operatorname{diag}(S_t)\sigma_t\,dW_t^Q,
$$

so the prices are [local martingales](../../../../../local-martingale.md) under $Q_T$.

Every admissible zero-initial-capital [self-financing portfolio](../../../../../self-financing-portfolio.md) has [portfolio wealth](../../../../../portfolio-wealth.md) which is therefore a $Q_T$-[local martingale](../../../../../local-martingale.md) bounded below by $-a$. The shifted process $X+a$ is a [nonnegative local martingale](../../../../../nonnegative-local-martingale.md), hence a [supermartingale](../../../../../supermartingale.md) by localization and the [Conditional Fatou lemma](../../../../../conditional-fatou-lemma.md). In particular $\mathbb E_{Q_T}X_T\leq0$. If the strategy were an [arbitrage](../../../../../arbitrage.md), nonnegativity of $X_T$ would force $X_T=0$ $Q_T$-almost surely. Equivalence of $P$ and $Q_T$ would then force $P(X_T>0)=0$, a contradiction. **The market has no admissible arbitrage on any finite horizon.** This proves the exclusion argument itself, rather than just asserting the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md).

For the deflated price calculation, let $\sigma_{t,i}$ denote the column vector whose transpose is the $i$th row of $\sigma_t$. The [Itô product rule](../../../../../ito-product-rule.md) includes the [quadratic covariation](../../../../../quadratic-covariation.md) term

$$
d[Z,S^i]_t=-Z_tS_t^i\sigma_{t,i}^T\lambda_t\,dt.
$$

Since $\sigma_{t,i}^T\lambda_t=\mu_t^i$, the full product equation is

$$
\begin{aligned}
d(Z_tS_t^i)&=Z_tS_t^i\left[(\mu_t^i-\sigma_{t,i}^T\lambda_t)dt+(\sigma_{t,i}-\lambda_t)^T\,dW_t\right]\\
&=Z_tS_t^i(\sigma_{t,i}-\lambda_t)^T\,dW_t.
\end{aligned}
$$

Localization makes the last [stochastic integral](../../../../../stochastic-integral.md) a true [martingale](../../../../../martingale-split.md) on each stopped interval, proving **each component of the deflated price vector is a local martingale under the original measure**. This is the [bounded-coefficient asset deflator](../../../../../bounded-coefficient-asset-deflator.md) identity; bounded volatility has not yet been used.

If $\sigma$ is bounded, then $\sigma_{t,i}-\lambda_t$ is bounded as well. Solving the last linear [stochastic differential equation](../../../../../stochastic-differential-equation.md) gives

$$
Z_tS_t^i=S_0^i\exp\left(\int_0^t(\sigma_{s,i}-\lambda_s)^T\,dW_s-\frac12\int_0^t|\sigma_{s,i}-\lambda_s|^2ds\right).
$$

The [Novikov condition](../../../../../novikov-s-condition.md) now holds for this [stochastic exponential](../../../../../doleans-dade-exponential.md) on every finite horizon, because its bracket is bounded by a deterministic constant times the horizon. Therefore

$$
\boxed{\mathbb E[Z_tS_t^i\mid\mathcal F_s]=Z_sS_s^i\quad(0\leq s\leq t),\qquad\mathbb E[Z_tS_t^i]=S_0^i.}
$$

**The entire deflated price vector is a true martingale when volatility is bounded.** This finite-horizon argument does not assert uniform integrability as time tends to infinity, which is not required. Integrable random initial prices can also be handled by the conditional martingale argument; without any integrability assumption on initial prices, a true-martingale assertion would not be meaningful.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

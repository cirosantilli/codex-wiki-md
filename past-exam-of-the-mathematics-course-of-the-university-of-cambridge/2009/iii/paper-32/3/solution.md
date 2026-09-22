<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On a fixed finite horizon, a [self-financing strategy](../../../../../self-financing-portfolio.md) consists of predictable [stock](../../../../../stock.md) holdings $h^i$, integrable against the price processes, and a [bank account](../../../../../bank-account.md) holding $h^0$. Its wealth and gains satisfy

$$
X_t=h_t^0B_t+\sum_{i=1}^dh_t^iS_t^i,\qquad dX_t=h_t^0dB_t+\sum_{i=1}^dh_t^idS_t^i.
$$

An [admissible trading strategy](../../../../../admissible-trading-strategy.md) has discounted wealth $X_t/B_t$ bounded below by a deterministic constant throughout the horizon. With the bounded [short rate](../../../../../short-rate.md) in this part, an undiscounted deterministic lower bound is equivalent after adjusting the constant. An [arbitrage](../../../../../arbitrage.md) is an admissible zero-initial-cost strategy with $X_T\ge0$ almost surely and $\mathbb P(X_T>0)>0$.

Put $\mathbf1=(1,\ldots,1)^\top$ and define the [market price of risk](../../../../../market-price-of-risk.md)

$$
\lambda_t=\sigma_t^{-1}(\mu_t-r_t\mathbf1).
$$

The bounded coefficients and bounded inverse make $\lambda$ bounded. Define the [stochastic exponential](../../../../../doleans-dade-exponential.md)

$$
L_t=\exp\left(-\int_0^t\lambda_s\cdot dW_s-\frac12\int_0^t\lVert\lambda_s\rVert^2ds\right).
$$

The [Novikov condition](../../../../../novikov-s-condition.md) states that $\mathbb E\exp(\tfrac12\int_0^T\lVert\lambda_s\rVert^2ds)<\infty$ makes this exponential a true [martingale](../../../../../martingale-split.md) with expectation one. Boundedness verifies the condition. Therefore $dQ=L_TdP$ defines an equivalent probability measure. The [Girsanov theorem](../../../../../girsanov-theorem.md) states that

$$
W_t^Q=W_t+\int_0^t\lambda_sds
$$

is a $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md) under $Q$. Substituting into the asset equations gives

$$
\frac{dS_t^i}{S_t^i}=r_tdt+\sum_j\sigma_t^{ij}dW_t^{Q,j},\qquad
\frac{d(S_t^i/B_t)}{S_t^i/B_t}=\sum_j\sigma_t^{ij}dW_t^{Q,j}.
$$

Thus $Q$ is an [equivalent local martingale measure](../../../../../equivalent-local-martingale-measure.md). The sufficient direction of the [fundamental theorem of asset pricing](../../../../../fundamental-theorem-of-asset-pricing.md) says that such a measure excludes [arbitrage](../../../../../arbitrage.md) among admissible [self-financing strategies](../../../../../self-financing-portfolio.md). Here the reason can be seen directly: $X/B$ is a [local martingale](../../../../../local-martingale.md) under $Q$, and its lower bound makes it a [supermartingale](../../../../../supermartingale.md). Consequently $X_0=0$ implies $\mathbb E_Q[X_T/B_T]\le0$, incompatible with the nonnegative terminal payoff of an [arbitrage](../../../../../arbitrage.md). Therefore **the bounded-inverse market has no [arbitrage](../../../../../arbitrage.md)**.

For the requested [law of one price](../../../../../law-of-one-price.md) counterexample, take a broader continuous-time local-martingale model on $[0,T]$. Let $X$ be a [Brownian motion](../../../../../brownian-motion-split.md), let $\tau=\inf\{u\ge0:X_u=-1\}$, and set $q(t)=t/(T-t)$ for $t<T$. Define

$$
\boxed{B_t=1,\qquad S_t=2+X_{q(t)\wedge\tau}\ (t<T),\qquad S_T=1.}
$$

The given hitting-time fact gives $\tau<\infty$ almost surely. The corresponding physical hitting time is $T\tau/(1+\tau)<T$, so $S$ reaches one and then stays one. In particular it is continuous at maturity and $S_t\ge1$.

For a rigorous closed-horizon localization, stop additionally when $S$ hits $n+2$, or at $T$ if it never does. The stopped process is [Brownian motion](../../../../../brownian-motion-split.md) stopped on first exiting $(-1,n)$ and subjected to the deterministic clock; it is a bounded [martingale](../../../../../martingale-split.md), including at $T$. The stopping times increase to $T$, since every Brownian path on the finite random interval $[0,\tau]$ has a finite maximum. Thus $S$ is a positive [local martingale](../../../../../local-martingale.md) on the whole horizon. With the time-changed Brownian filtration, the original probability measure is an [equivalent local martingale measure](../../../../../equivalent-local-martingale-measure.md). The admissible-wealth [supermartingale](../../../../../supermartingale.md) argument above proves **no admissible [arbitrage](../../../../../arbitrage.md)**.

Nevertheless $S_T=B_T=1$ while $S_0=2\ne B_0=1$, so **the [law of one price](../../../../../law-of-one-price.md) fails**. Shorting one share and buying two units of cash has zero initial cost and terminal gain one, but its wealth is $2-S_t$. It has no deterministic lower bound: for every $n$, the probability of [Brownian motion](../../../../../brownian-motion-split.md) hitting $n$ before $-1$ is $1/(n+1)>0$, obtained by optional stopping of the bounded stopped [Brownian motion](../../../../../brownian-motion-split.md). That apparently profitable strategy is therefore inadmissible. The counterexample deliberately uses a [strict local martingale](../../../../../strict-local-martingale.md); the bounded-coefficient class in the first part has true discounted asset [martingales](../../../../../martingale-split.md) and does satisfy the [law of one price](../../../../../law-of-one-price.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

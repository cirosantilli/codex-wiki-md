<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take a non-dividend-paying [stock](../../../../../stock.md) with physical dynamics $dS_t=\mu S_tdt+\sigma S_tdW_t$ and [continuous-time bank account](../../../../../continuous-time-bank-account.md) $B_t=e^{\rho t}$. Write $T=t_0$ and assume the candidate claim price $p(x,t)$ is $C^{2,1}$ before maturity, with enough growth control for the hedge to be admissible. The terminal condition is $p(x,T)=f(x)$.

The [Itô formula](../../../../../ito-s-lemma.md) gives the claim's price change

$$
dp(S_t,t)=\left(p_t+\mu S_tp_x+\tfrac12\sigma^2S_t^2p_{xx}\right)dt+\sigma S_tp_x\,dW_t.
$$

A [self-financing portfolio](../../../../../self-financing-portfolio.md) worth $p$ with $\Delta$ shares has bank-account value $p-\Delta S_t$. Its gain is

$$
\Delta\,dS_t+\rho(p-\Delta S_t)dt
=\{\mu\Delta S_t+\rho(p-\Delta S_t)\}dt+\sigma\Delta S_t\,dW_t.
$$

To replicate the claim, the Brownian coefficients must agree, forcing the [delta hedge](../../../../../delta-hedge.md) $\Delta=p_x$. Equating the remaining [drift](../../../../../drift-coefficient.md) coefficients cancels the physical [drift](../../../../../drift-coefficient.md) $\mu$ and yields

$$
\boxed{p_t+\rho xp_x+\tfrac12\sigma^2x^2p_{xx}-\rho p=0,\qquad p(x,T)=f(x).}
$$

The cancellation explains why the [Black-Scholes equation](../../../../../black-scholes-equation.md) contains the [interest rate](../../../../../interest-rate.md), not the physical [stock](../../../../../stock.md) [drift](../../../../../drift-coefficient.md). Conversely, if an admissible solution of this equation is given, holdings $p_x$ in the [stock](../../../../../stock.md) and $(p-xp_x)/B_t$ in the [bank account](../../../../../bank-account.md) have value $p$ and gains exactly $dp$. They are therefore a [self-financing portfolio](../../../../../self-financing-portfolio.md) replicating the terminal payoff. Absence of [arbitrage](../../../../../arbitrage.md) forces the claim to have this price. Merely decomposing the current value into arbitrary holdings would not justify self-financing; the gain identity and [delta hedge](../../../../../delta-hedge.md) are essential.

Now suppose the claim holder receives the cash rate $k(S_t,t)$ before $T$. The price $p$ is the ex-dividend value, so its total gain is $dp+kdt$. The replicating [portfolio](../../../../../investment-portfolio.md) pays the same amounts out of its wealth, with no external injections. Thus its gain identity is

$$
dp+k(S_t,t)dt=\Delta\,dS_t+\rho(p-\Delta S_t)dt.
$$

Again the Brownian coefficients force $\Delta=p_x$. Comparing [drifts](../../../../../drift-coefficient.md) now gives the [Black-Scholes equation with claim dividends](../../../../../black-scholes-equation-with-claim-dividends.md):

$$
\boxed{p_t+\rho xp_x+\tfrac12\sigma^2x^2p_{xx}-\rho p+k(x,t)=0,\qquad p(x,T)=f(x).}
$$

In particular the cash-flow source has a positive sign in the left-hand side. It is not an underlying-stock dividend yield and does not replace the [drift](../../../../../drift-coefficient.md) $\rho x$ by a dividend-adjusted [drift](../../../../../drift-coefficient.md).

For another justification, under the [risk-neutral measure](../../../../../risk-neutral-measure.md) $Q$, discount the claim's cum-dividend gain. The [Itô formula](../../../../../ito-s-lemma.md) shows that

$$
d\left(e^{-\rho t}p(S_t,t)+\int_0^t e^{-\rho u}k(S_u,u)\,du\right)
=e^{-\rho t}\sigma S_tp_x\,dW_t^Q
$$

exactly when the displayed equation holds. Subject to the usual [integrability](../../../../../integrability.md) making this a true [martingale](../../../../../martingale-split.md), [conditional expectation](../../../../../conditional-expectation.md) at maturity gives

$$
p(x,t)=\mathbb E_Q\left[e^{-\rho(T-t)}f(S_T)+\int_t^T e^{-\rho(u-t)}k(S_u,u)\,du\,\middle|\,S_t=x\right].
$$

Positive interim payments therefore add positive value, which also checks the source sign. For instance, a constant payment rate $k_0$ and zero terminal payoff have price $k_0(1-e^{-\rho(T-t)})/\rho$, interpreted as $k_0(T-t)$ at $\rho=0$; substitution satisfies $p_t-\rho p+k_0=0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

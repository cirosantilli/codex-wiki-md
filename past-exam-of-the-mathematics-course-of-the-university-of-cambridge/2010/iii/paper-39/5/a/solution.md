<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Black-Scholes equation](../../../../../../black-scholes-equation.md) with the claim's terminal condition $V(T,s)=g(s)$:

$$
V_t+rsV_s+\frac12\sigma^2s^2V_{ss}-rV=0.
$$

For $t<T$, the [Itô formula](../../../../../../ito-s-lemma.md) under the physical measure gives

$$
dV(t,S_t)=\left(rV(t,S_t)+(\mu-r)S_tV_s(t,S_t)\right)dt
+\sigma S_tV_s(t,S_t)\,dW_t.
$$

Choose the [delta hedge](../../../../../../delta-hedge.md) and its bank-account holding by

$$
\boxed{\pi_t=V_s(t,S_t),\qquad
\phi_t=\frac{V(t,S_t)-S_tV_s(t,S_t)}{B_t}.}
$$

Their portfolio value is $V(t,S_t)$, and

$$
\phi_t\,dB_t+\pi_t\,dS_t
=\left(rV+(\mu-r)S_tV_s\right)dt+\sigma S_tV_s\,dW_t
=dV(t,S_t).
$$

Thus the portfolio is [self-financing](../../../../../../self-financing-portfolio.md) and, with initial capital $V(0,S_0)$, has terminal wealth $g(S_T)$.

Localizing to compact stock-price intervals and times below $T$ justifies these stochastic integrals from the classical smoothness of $V$. The extension to maturity also follows from boundedness. Under the [Risk-neutral measure for the Black-Scholes model](../../../../../../risk-neutral-measure-for-the-black-scholes-model.md), discounted $V(t,S_t)$ is a bounded [local martingale](../../../../../../local-martingale.md), hence a true square-integrable [martingale](../../../../../../martingale-split.md). Its quadratic variation has finite expectation, so the stock-integral coefficient is square integrable through $T$. Equivalence of measures preserves its almost-sure finiteness, and the physical drift integral is finite by [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md). The terminal limit is $g(S_T)$.

Finally, $B_t=B_0e^{rt}$ is bounded away from zero on this finite horizon, and bounded $V$ makes $V(t,S_t)/B_t$ bounded below by a deterministic constant. The hedge is therefore an [admissible trading strategy](../../../../../../admissible-trading-strategy.md). **The displayed holdings replicate the payoff admissibly**, even if the bounded payoff can be negative.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

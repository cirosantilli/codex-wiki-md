<h1 id="29j/solution">Solution</h1>

↑ **Parent:** [29J](../29j.md)

A standard [Brownian motion](../../../../../brownian-motion-split.md) $W_t$ starts at zero, has continuous sample paths, and has independent increments $W_t-W_s\sim N(0,t-s)$ for $0\le s<t$. The [Black-Scholes model](../../../../../black-scholes-model.md) assumes a frictionless market permitting continuous, self-financing trading and short selling, a bank account $B_t=e^{rt}$ at constant interest rate, and a non-dividend-paying asset

$$
dS_t=\mu S_t\,dt+\sigma S_t\,dW_t,\qquad S_0>0,\quad\sigma>0,
$$

with constant coefficients and no arbitrage.

For an option price $C(S,t)$, [Itô's formula](../../../../../ito-s-lemma.md) gives diffusion coefficient $\sigma SC_S$. Holding $C_S$ units of the asset hedges this diffusion. The hedged portfolio has value $C-SC_S$ and instantaneous gain $(C_t+\tfrac12\sigma^2S^2C_{SS})dt$, so no arbitrage requires

$$
C_t+\frac12\sigma^2S^2C_{SS}+rSC_S-rC=0,\qquad C(S,T)=(S-K)^+.
$$

Equivalently, the [risk-neutral measure](../../../../../risk-neutral-measure.md) makes $e^{-rt}S_t$ a martingale and gives the solution $C(S_0,0)=e^{-rT}\mathbb E_Q(S_T-K)^+$. Under that measure,

$$
S_T=S_0\exp\!\left((r-\sigma^2/2)T+\sigma\sqrt T\,Z\right),\qquad Z\sim N(0,1).
$$

Put $d_2=[\log(S_0/K)+(r-\sigma^2/2)T]/(\sigma\sqrt T)$ and $d_1=d_2+\sigma\sqrt T$. Then $\mathbb P_Q(S_T>K)=\Phi(d_2)$, and completing the square in the normal integral gives $\mathbb E_Q[S_T\mathbf1_{S_T>K}]=S_0e^{rT}\Phi(d_1)$. Therefore the [Black-Scholes formula](../../../../../black-scholes-formula.md) is

$$
\boxed{C_0=S_0\Phi(d_1)-Ke^{-rT}\Phi(d_2).}
$$

Here $K>0$; a zero strike has value $S_0$ directly.

For the [forward-start call option](../../../../../forward-start-call-option.md), condition at the strike-fixing time $t$. Given $\mathcal F_t$, the remaining asset-price ratio has the same lognormal law over $\tau=T-t$, independently of past increments. Thus its time-$t$ value is

$$
C_t=S_t\left[\Phi\!\left(\frac{(r+\sigma^2/2)\sqrt\tau}{\sigma}\right)-e^{-r\tau}\Phi\!\left(\frac{(r-\sigma^2/2)\sqrt\tau}{\sigma}\right)\right].
$$

Since $\mathbb E_Q(e^{-rt}S_t)=S_0$, conditioning once more yields

$$
\boxed{C_0=S_0\left[\Phi\!\left(\frac{(r+\sigma^2/2)\sqrt{T-t}}\sigma\right)-e^{-r(T-t)}\Phi\!\left(\frac{(r-\sigma^2/2)\sqrt{T-t}}\sigma\right)\right].}
$$

The strike is random before $t$; inserting an unknown $S_t$ as a fixed strike at time zero would miss the conditioning step.

## ↑ Ancestors (10)

1. [29J](../29j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

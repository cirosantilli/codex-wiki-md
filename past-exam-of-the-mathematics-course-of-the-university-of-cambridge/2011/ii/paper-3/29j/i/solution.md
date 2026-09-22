<h1 id="29j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A standard [Brownian motion](../../../../../../brownian-motion-split.md) starts at zero, has continuous sample paths and independent increments, with $W_t-W_s\sim N(0,t-s)$ for $0\leq s<t$.

Assume $S_0,K,T>0$ and $\sigma>0$; changing the sign of $\sigma$ just changes the sign of Brownian motion. [Itô formula](../../../../../../ito-s-lemma.md) gives $dS_t=S_t[(\mu+\sigma^2/2)dt+\sigma\,dW_t]$. In the complete [Black-Scholes model](../../../../../../black-scholes-model.md), the [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) theorem prices an integrable payoff $Y$ by $e^{-rT}\mathbb E_QY$, where the discounted asset is a martingale. [Girsanov theorem](../../../../../../girsanov-theorem.md) therefore replaces the logarithmic drift by $r-\sigma^2/2$:

$$
\log S_T=\log S_0+(r-\sigma^2/2)T+\sigma\sqrt T\,Z,\qquad Z\sim N(0,1)\text{ under }Q.
$$

Let $d_2=[\log(S_0/K)+(r-\sigma^2/2)T]/(\sigma\sqrt T)$ and $d_1=d_2+\sigma\sqrt T$. The exercise event is $Z>-d_2$. Completing the square in the Gaussian integral yields

$$
\mathbb E[e^{aZ}\mathbf1_{\{Z>b\}}]=e^{a^2/2}\Phi(a-b).
$$

Consequently $\mathbb P_Q(S_T>K)=\Phi(d_2)$ and $\mathbb E_Q[S_T\mathbf1_{\{S_T>K\}}]=S_0e^{rT}\Phi(d_1)$. Thus the [European call option](../../../../../../european-call-option.md) price is

$$
\boxed{C_0=S_0\Phi(d_1)-Ke^{-rT}\Phi(d_2).}
$$

The physical drift $\mu$ disappears because the price is obtained under the martingale measure. If $\sigma=0$ in an arbitrage-free deterministic model, $S_t=S_0e^{rt}$ and the formula is interpreted by its zero-volatility limit.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [29J](../../29j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

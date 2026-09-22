<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Phi$ denote the standard [normal distribution](../../../../../../normal-distribution.md) [cumulative distribution function](../../../../../../cumulative-distribution-function.md), and $\phi$ its density. Put $\tau=T-t$. For $K>0$ and $t<T$, define

$$
d_1=\frac{\log(S_t/K)+(r+\sigma^2/2)\tau}{\sigma\sqrt\tau},\qquad d_2=d_1-\sigma\sqrt\tau.
$$

Under the [risk-neutral measure](../../../../../../risk-neutral-measure.md), conditional on $\mathcal F_t$,

$$
S_T=S_t\exp\bigl((r-\sigma^2/2)\tau+\sigma\sqrt\tau\,Z\bigr),\qquad Z\sim N(0,1).
$$

Thus $Q(S_T<K\mid\mathcal F_t)=\Phi(-d_2)$. The identity $e^{az}\phi(z)=e^{a^2/2}\phi(z-a)$ for the standard [Gaussian distribution](../../../../../../normal-distribution.md) [probability density function](../../../../../../probability-density-function.md) gives

$$
\mathbb E_Q[S_T\mathbf1_{\{S_T\geq K\}}\mid\mathcal F_t]=S_te^{r\tau}\Phi(d_1).
$$

Split the payout according to whether the stock exceeds the floor and discount. The [risk-neutral pricing](../../../../../../risk-neutral-pricing.md) process is

$$
\boxed{\xi_t=V(t,S_t)=S_t\Phi(d_1)+Ke^{-r(T-t)}\Phi(-d_2),\qquad \xi_T=\max(K,S_T).}
$$

Its discounted value is $\mathbb E_Q[\xi_T/B_T\mid\mathcal F_t]$, a true [martingale](../../../../../../martingale-split.md). Thus adding this asset preserves the [equivalent martingale measure](../../../../../../risk-neutral-measure.md) and gives no [arbitrage](../../../../../../arbitrage.md). This is the [guaranteed terminal stock floor in the Black-Scholes model](../../../../../../guaranteed-terminal-stock-floor-in-the-black-scholes-model.md). For $K\leq0$, positivity of the stock makes the claim simply $S_T$, and the price is $\xi_t=S_t$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

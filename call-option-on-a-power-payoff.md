# Call option on a power payoff

↑ **Parent:** [Power payoff in the Black-Scholes model](power-payoff-in-the-black-scholes-model.md)

For $p>0$ in a non-dividend-paying [Black-Scholes model](black-scholes-model.md), the replicating price of the terminal power payoff $S_T^p$ is

$$
V_t^{(p)}=S_t^p\exp\left[\left((p-1)r+\tfrac12p(p-1)\sigma^2\right)(T-t)\right].
$$

Its [self-financing portfolio](self-financing-portfolio.md) holds $pV_t^{(p)}/S_t$ shares and bank wealth $(1-p)V_t^{(p)}$. [Itô's formula](ito-s-lemma.md) gives physical drift $p\mu-(p-1)r$ and volatility $p\sigma$ for this replicating asset; its risk-neutral drift is $r$.

Since $V_T^{(p)}=S_T^p$, the payoff $(S_T^p-K)^+$ is a [European call option](european-call-option.md) on this replicating asset. The [Black-Scholes formula](black-scholes-formula.md) gives the displayed price with $\tau=T-t$ and $d_2=d_1-p\sigma\sqrt\tau$. Using the raw process $S_t^p$ as a non-dividend-paying underlying would miss its time-dependent replication factor.

## ↑ Ancestors (8)

1. [Power payoff in the Black-Scholes model](power-payoff-in-the-black-scholes-model.md)
2. [Risk-neutral measure for the Black-Scholes model](risk-neutral-measure-for-the-black-scholes-model.md)
3. [Black-Scholes model](black-scholes-model.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-martingales-and-financial-mathematics-course-of-the-university-of-oxford/2011/b/5/e/solution.md)

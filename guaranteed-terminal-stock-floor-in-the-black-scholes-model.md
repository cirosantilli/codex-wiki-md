# Guaranteed terminal stock floor in the Black-Scholes model

↑ **Parent:** [Black-Scholes model](black-scholes-model.md)

The claim $\max(K,S_T)$ for $K>0$ combines a guaranteed cash floor with a [European call option](european-call-option.md), equivalently a stock with a put. In the [Black-Scholes model](black-scholes-model.md), for $\tau=T-t>0$, its price is $V=S_t\Phi(d_1)+Ke^{-r\tau}\Phi(-d_2)$, where $d_1=[\log(S_t/K)+(r+\sigma^2/2)\tau]/(\sigma\sqrt\tau)$ and $d_2=d_1-\sigma\sqrt\tau$. Under the risk-neutral lognormal law, the truncated stock moment is $S_te^{r\tau}\Phi(d_1)$ and the probability of ending below the floor is $\Phi(-d_2)$, proving the price. Its [option delta](option-delta.md) is $\Phi(d_1)$, since $S_t\phi(d_1)=Ke^{-r\tau}\phi(d_2)$ cancels the derivative terms. The [replicating strategy](replicating-strategy.md) holds that many stock units and $Ke^{-r\tau}\Phi(-d_2)/B_t$ bank-account units.

## ↑ Ancestors (6)

1. [Black-Scholes model](black-scholes-model.md)
2. [Mathematical finance](mathematical-finance-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39/4/ii/solution.md)

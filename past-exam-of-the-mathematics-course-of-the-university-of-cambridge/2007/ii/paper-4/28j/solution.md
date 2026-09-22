<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

In the [Black-Scholes model](../../../../../black-scholes-model.md), the stock follows geometric Brownian motion $dS=\mu S\,dt+\sigma S\,dW$, with constant volatility, and a risk-free account earns constant rate $r$. Frictionless continuous self-financing trading and no arbitrage lead to risk-neutral drift $r$. With $\tau=T-t$, risk-neutral lognormality gives

$$
\boxed{V(t,s)=e^{-r\tau}\Phi(d_2),\qquad
 d_2=\frac{\log(s/K)+(r-\sigma^2/2)\tau}{\sigma\sqrt\tau}.}
$$

This is the [Black-Scholes digital option formula](../../../../../black-scholes-digital-option-formula.md), obtained by discounting $P(S_T>K)$, not the stock-weighted probability of an ordinary call. Differentiation gives the [Delta hedge](../../../../../delta-hedge.md)

$$
\boxed{\Delta(t,s)=\frac{e^{-r\tau}\varphi(d_2)}{s\sigma\sqrt\tau},}
$$

where $\Phi,\varphi$ are the standard [normal distribution](../../../../../normal-distribution.md) and density. At fixed $s\ne K$, the density term decays faster than $\tau^{-1/2}$ grows, so delta tends to zero. At $s=K$, $d_2\to0$ and $\Delta\sim[K\sigma\sqrt{2\pi\tau}]^{-1}$ diverges. Thus a narrowing, increasingly large delta spike forms around the strike. The terminal payoff is discontinuous: frequent large hedge adjustments near the strike, transaction costs, jumps, discrete trading, and small model or price errors make practical replication difficult. A fixed path avoiding the strike and the at-the-strike limit need not behave alike.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

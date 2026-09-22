<h1 id="b/5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For a [call option on a power payoff](../../../../../call-option-on-a-power-payoff.md), the replicating asset $V$ from part (c) has $V_T=S_T^3$, volatility $3\sigma$, and risk-neutral drift $r$. The new payoff is therefore a [European call option](../../../../../european-call-option.md) on $V$, with strike $K$. Applying the given [Black-Scholes formula](../../../../../black-scholes-formula.md) gives

$$
\boxed{C_t=V_t\Phi(D_1)-Ke^{-r\tau}\Phi(D_2),\qquad
D_1=\frac{\log(V_t/K)+(r+9\sigma^2/2)\tau}{3\sigma\sqrt\tau},\quad
D_2=D_1-3\sigma\sqrt\tau.}
$$

Here $V_t=S_t^3e^{(2r+3\sigma^2)\tau}$. Equivalently $D_1=[\log(S_t^3/K)+(3r+15\sigma^2/2)\tau]/(3\sigma\sqrt\tau)$. It is the price process $V_t$, rather than the raw power $S_t^3$, that serves as the self-financing underlying for this application.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

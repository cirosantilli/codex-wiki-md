<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A self-financing replicating strategy must fund both the claim's price change and its outgoing cash flow:

$$
dV_t+q_tS_t\,dt=\Delta_t\,dS_t+\beta_t\,dB_t,\qquad
V_t=\Delta_tS_t+\beta_tB_t.
$$

Apply [Itô's formula](../../../../../ito-s-lemma.md) to $V(t,S_t)$. Matching the diffusion gives $\Delta=V_s$. Matching drift and eliminating $\beta B=V-sV_s$ gives the [Black-Scholes equation with claim dividends](../../../../../black-scholes-equation-with-claim-dividends.md)

$$
\boxed{V_t+\tfrac12\sigma^2s^2V_{ss}+rsV_s-rV+q_ts=0,\qquad
V(T,s)=\Psi(s).}
$$

The physical drift cancels because stock risk is hedged. The cash-flow term has a plus sign because it is a payment to the holder.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

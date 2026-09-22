<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an ex-dividend stock, holding $\Delta$ shares earns both $\Delta\,dS$ and the dividend gain $\Delta\delta S\,dt$. Freeze $\Delta=V_S$ locally in a self-financing hedge that is long the claim and short these shares. [Itô's formula](../../../../../ito-s-lemma.md) cancels its Brownian exposure, leaving drift $V_t+\tfrac12\sigma^2S^2V_{SS}-\delta SV_S$. Its value is $V-SV_S$, so absence of arbitrage requires this drift to equal $r(V-SV_S)$. Rearrangement gives the [Black-Scholes equation with continuous stock dividends](../../../../../black-scholes-equation-with-continuous-stock-dividends.md):

$$
V_t+(r-\delta)SV_S+\tfrac12\sigma^2S^2V_{SS}-rV=0.
$$

With the given parameters,

$$
\boxed{V_t+0.04SV_S+0.02S^2V_{SS}-0.05V=0,\qquad V(T,S)=\Psi(S).}
$$

The physical drift $0.1$ cancels because the hedge removes the stock-price risk; the dividend payment remains in the stock's total gain.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
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

<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The commodity's total gain from holding one unit is $dS-\delta\,dt$, because the storage cost is a fixed cash rate, not a proportional dividend yield. Form a locally self-financing delta hedge long the derivative and short $\Delta=V_S$ units of the commodity. [Itô's formula](../../../../../ito-s-lemma.md) eliminates Brownian risk and leaves drift

$$
V_t+\tfrac12\sigma^2S^2V_{SS}+\delta V_S.
$$

Its value is $V-SV_S$, so absence of arbitrage makes that drift equal to $r(V-SV_S)$. Therefore the [Black-Scholes equation with constant cash storage costs](../../../../../black-scholes-equation-with-constant-cash-storage-costs.md) is

$$
\boxed{V_t+(rS+\delta)V_S+\tfrac12\sigma^2S^2V_{SS}=rV,\qquad V(T,S)=\Psi(S).}
$$

The cash cost enters as $\delta V_S$, rather than as $\delta SV_S$, because one unit costs $\delta$ per unit time regardless of its current price.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

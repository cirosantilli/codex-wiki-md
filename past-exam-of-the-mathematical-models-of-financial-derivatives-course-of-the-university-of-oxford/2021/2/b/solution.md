<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Buy $1/F_0^T$ shares and take a short [forward contract](../../../../forward-contract.md) for $1/F_0^T$ shares at delivery price $F_0^T$. The forward has zero initial value, and the combined terminal payoff is

$$
\frac{S_T}{F_0^T}+\frac{F_0^T-S_T}{F_0^T}=1.
$$

Therefore the [synthetic zero-coupon bond](../../../../synthetic-zero-coupon-bond.md) has initial price

$$
\boxed{P(0,T)=\frac{S_0}{F_0^T}.}
$$

Its implied continuously compounded maturity yield is $r_T=T^{-1}\log(F_0^T/S_0)>0$.

To replicate a constant-rate [risk-free asset](../../../../risk-free-asset.md) throughout the interval, the market must support dynamically coherent discounting, not just this one terminal payment. A sufficient condition is that for all $0\leq t\leq u\leq T$ the fair forward prices satisfy $F_t^u=S_te^{r(u-t)}$ for the same deterministic $r>0$, with the required stock/forward positions tradable and no intervening payments. Then $P(t,u)=S_t/F_t^u=e^{-r(u-t)}$, and a suitably scaled fixed-maturity [zero-coupon bond](../../../../zero-coupon-bond.md) grows deterministically as $e^{rt}$. A single initial forward quote does not establish these intermediate-time conditions; even a flat initial yield curve need not imply deterministic future rates.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

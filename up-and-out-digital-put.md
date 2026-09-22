# Up-and-out digital put

↑ **Parent:** [Barrier option](barrier-option.md)

A [digital put option](digital-put-option.md) extinguished if the [stock](stock.md) reaches an upper barrier $B$. Under the dividend-free [Black-Scholes model](black-scholes-model.md), conditional on not having hit the barrier before the current time, let $0<S<B$, $\tau=T-t>0$, $m=\min(K,B)$, $\gamma=1-2r/\sigma^2$, and

$$
D_m(S,t)=e^{-r\tau}\Phi\!\left(\frac{\log(m/S)-(r-\sigma^2/2)\tau}{\sigma\sqrt\tau}\right).
$$

Then its price is

$$
H(S,t)=D_m(S,t)-(S/B)^\gamma D_m(B^2/S,t).
$$

The [Black-Scholes reflection symmetry](black-scholes-reflection-symmetry.md) proves the pricing equation, and the two terms cancel at $S=B$. At expiry the reflected argument is above $B\geq m$, so its payoff is zero, while $S<m$ is equivalent to $S<K$ inside the alive region. Thus the correct free strike is capped at the barrier. For $K\geq B$, the value is the discounted upper-barrier survival probability, independent of $K$, as for a [barrier digital put](barrier-digital-put.md). For $K>B$ its terminal data have a corner discontinuity at the absorbing barrier. Set the price to zero after a hit; the reflected expression on the other side is not a valid contract value.

## ↑ Ancestors (8)

1. [Barrier option](barrier-option.md)
2. [Contingent claim](contingent-claim.md)
3. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2015/3/b/iv/solution.md)

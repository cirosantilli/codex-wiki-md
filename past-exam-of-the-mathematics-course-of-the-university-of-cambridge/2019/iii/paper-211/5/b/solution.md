<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The one-period [spot interest rate](../../../../../../spot-interest-rate.md) is defined by

$$
1+r_t=\frac1{P_t^{t+1}},
$$

and the [bank account](../../../../../../bank-account.md) by

$$
B_0=1,
\qquad
B_t=\prod_{s=0}^{t-1}(1+r_s).
$$

A probability measure $Q$ equivalent to the physical measure is a [risk-neutral measure](../../../../../../risk-neutral-measure.md) when every discounted [zero-coupon bond](../../../../../../zero-coupon-bond.md) price

$$
\frac{P_t^T}{B_t},\qquad0\leq t\leq T,
$$

is a $Q$-martingale. Equivalently,

$$
P_t^T=B_t\mathbb E^Q[B_T^{-1}\mid\mathcal F_t].
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

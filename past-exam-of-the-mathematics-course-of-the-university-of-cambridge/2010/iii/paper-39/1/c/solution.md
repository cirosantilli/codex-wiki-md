<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $q(T)$ denote the original [zero-coupon bond](../../../../../../zero-coupon-bond.md) price $P(0,T)$ computed above. A deterministic shift $h_t$ of the [short rate](../../../../../../short-rate.md), with $h_0=0$, gives $\widehat r_t=r_t+h_t$. Subtracting the two recursions shows that the required added drift is

$$
\alpha_t=h_t-\beta h_{t-1}.
$$

Since the shift is nonrandom, the new [discount factor](../../../../../../discount-factor.md) differs by $\exp(-\sum_{s=1}^Th_s)$, and hence $\widehat P(0,T)=q(T)\exp(-\sum_{s=1}^Th_s)$.

For [deterministic calibration of an autoregressive short rate](../../../../../../deterministic-calibration-of-an-autoregressive-short-rate.md), define

$$
d_T=\log q(T)-\log p(T),\qquad d_0=0,\qquad h_T=d_T-d_{T-1}\quad(T\geq1).
$$

All these quantities are finite. The telescoping sum $\sum_{s=1}^Th_s=d_T$ gives $\widehat P(0,T)=p(T)$. Explicitly,

$$
\boxed{\alpha_1=d_1,\qquad
\alpha_T=d_T-(1+\beta)d_{T-1}+\beta d_{T-2}\quad(T\geq2).}
$$

These constants fit every maturity simultaneously. Each successive maturity fixes $h_T$ uniquely, so the deterministic calibration is also unique with the prescribed $r_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

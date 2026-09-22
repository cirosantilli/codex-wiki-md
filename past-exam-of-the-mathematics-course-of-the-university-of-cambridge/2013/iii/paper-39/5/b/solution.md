<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A unit [zero-coupon bond](../../../../../../zero-coupon-bond.md) pays one at its maturity, so $P_t(t)=1$. Monotonicity in maturity gives $P_t(t+1)\le1$. Using the [state-price density](../../../../../../state-price-density.md) representation with $T=t+1$,

$$
\boxed{\mathbb E(Z_{t+1}\mid\mathcal F_t)=Z_tP_t(t+1)\le Z_t.}
$$

The process is positive and integrable, as noted in part (a), and adapted. Thus it is a [supermartingale](../../../../../../supermartingale.md). Strictly decreasing maturity prices yield a strict one-step conditional inequality; weak decrease is already enough for the conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

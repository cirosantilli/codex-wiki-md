<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) curve determines the unit-face-value [zero-coupon bond](../../../../../../zero-coupon-bond.md) through $f(t,T)=-\partial_T\log P(t,T)$ and $P(t,t)=1$. Integrating in maturity gives

$$
\boxed{P(t,T)=\exp\left[-\int_t^Tf(t,u)du\right].}
$$

The diagonal is the [short rate](../../../../../../short-rate.md), $\boxed{r_t=f(t,t)}$, and the [continuous-time bank account](../../../../../../continuous-time-bank-account.md) has $B_t=\exp(\int_0^tr_sds)$ when $B_0=1$. Therefore the [discounted bond price martingale](../../../../../../discounted-bond-price-martingale.md) has value

$$
\boxed{Z_t(t,T)=B_t^{-1}P(t,T)
=\exp\left[-\int_0^tr_sds-\int_t^Tf(t,u)du\right].}
$$

Under the [risk-neutral measure](../../../../../../risk-neutral-measure.md) of the [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md), sufficiently integrable discounted bond prices are true [martingales](../../../../../../martingale-split.md); without that integrability their stochastic dynamics initially establish a local [martingale](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

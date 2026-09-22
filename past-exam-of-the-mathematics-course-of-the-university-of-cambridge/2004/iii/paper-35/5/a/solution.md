<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a unit-face [zero-coupon bond](../../../../../../zero-coupon-bond.md) with $P(T,T)=1$. Its continuously compounded [zero-coupon yield to maturity](../../../../../../zero-coupon-yield-to-maturity.md), [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md), and [short rate](../../../../../../short-rate.md) are

$$
\boxed{R(t,T)=-\frac{\log P(t,T)}{T-t},\qquad
f(t,T)=-\partial_T\log P(t,T),\qquad
r(t)=\lim_{T\downarrow t}R(t,T)=f(t,t).}
$$

The last equality assumes the appropriate maturity differentiability at the diagonal. Integration of the forward-rate definition and differentiation of the yield definition give

$$
P(t,T)=\exp\left[-\int_t^Tf(t,u)du\right]=e^{-(T-t)R(t,T)},\qquad
\boxed{R(t,T)=\frac1{T-t}\int_t^Tf(t,u)du,\quad f(t,T)=R(t,T)+(T-t)R_T(t,T).}
$$

At fixed observation time $t$, the [yield curve](../../../../../../yield-curve.md) plots this yield against maturity $T$; it describes today's discount prices at different horizons. Forward rates are extracted from these prices, not identified with the subsequent realized path of the [short rate](../../../../../../short-rate.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

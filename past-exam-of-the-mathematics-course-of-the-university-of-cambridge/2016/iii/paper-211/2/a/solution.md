<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [short rate](../../../../../../short-rate.md) is the limiting [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) at the present maturity. The continuously compounded [zero-coupon bond](../../../../../../zero-coupon-bond.md) price is obtained by integrating the [instantaneous forward rate](../../../../../../instantaneous-forward-rate.md) curve in its maturity variable. **Both requested relations are**

$$
\boxed{r_t=f(t,t),\qquad
P(t,T)=\exp\!\left(-\int_t^T f(t,u)\,du\right).}
$$

In particular $P(T,T)=1$, and $f(t,T)=-\partial_T\log P(t,T)$. The [short rate](../../../../../../short-rate.md) here is instantaneous, rather than the one-period rate used in a discrete-time [bank account](../../../../../../bank-account.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

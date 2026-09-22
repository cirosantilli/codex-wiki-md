<h1 id="b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), the same second-moment formula uses drift $r$. Discounting the [power option](../../../../../power-option.md) payoff therefore gives

$$
V(t,s)=e^{-r(T-t)}\mathbb E[S_T^2\mid S_t=s]
=\boxed{s^2e^{(r+\sigma^2)(T-t)}}.
$$

Let $a(t)=e^{(r+\sigma^2)(T-t)}$ and $B_t=e^{rt}$. The [delta hedging](../../../../../delta-hedge.md) portfolio holds

$$
\boxed{\Delta_t=2a(t)S_t\ \text{stock units},\qquad
\beta_t=-\frac{a(t)S_t^2}{B_t}\ \text{bank-account units}.}
$$

Its wealth is $\Delta_tS_t+\beta_tB_t=a(t)S_t^2=V_t$. To verify self financing, Itô's formula gives

$$
dV_t=(2\mu-r)V_t\,dt+2\sigma V_t\,dW_t
=\Delta_t\,dS_t+\beta_t\,dB_t.
$$

At maturity the wealth is $S_T^2$, completing replication.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

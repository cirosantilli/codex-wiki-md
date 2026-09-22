<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A stock holding receives both its price change and [dividend](../../../../../dividend.md), so its total gains are $dS+\delta Sdt$. The [replicating portfolio](../../../../../replicating-strategy.md) therefore satisfies

$$
dV_\delta=\Delta(dS+\delta Sdt)+r(V_\delta-\Delta S)dt.
$$

[Itô's formula](../../../../../ito-s-lemma.md) and the hedge $\Delta=(V_\delta)_S$ cancel the Brownian risk. Comparing drifts gives

$$
\boxed{(V_\delta)_t+\tfrac12\sigma^2S^2(V_\delta)_{SS}
+(r-\delta)S(V_\delta)_S-rV_\delta=0,\quad
V_\delta(T,S)=\Psi(S).}
$$

To verify the claimed transformation, put $x=Se^{-\delta(T-t)}$ and set $U(t,S)=V_0(t,x)$. Then $x_t=\delta x$, $S U_S=x(V_0)_x$ and $S^2U_{SS}=x^2(V_0)_{xx}$. The [dividend](../../../../../dividend.md) operator applied to $U$ becomes

$$
(V_0)_t+\delta x(V_0)_x
+\tfrac12\sigma^2x^2(V_0)_{xx}
+(r-\delta)x(V_0)_x-rV_0=0
$$

by the zero-dividend PDE. At maturity $x=S$, so the [contingent claim payoff](../../../../../contingent-claim-payoff.md) also agrees. Uniqueness in the pricing class proves

$$
\boxed{V_\delta(t,S)=V_0(t,Se^{-\delta(T-t)}).}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

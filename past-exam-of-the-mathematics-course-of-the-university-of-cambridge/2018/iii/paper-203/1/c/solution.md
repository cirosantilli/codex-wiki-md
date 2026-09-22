<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work with a locally growing [Loewner chain](../../../../../../loewner-chain.md) started at $0$, with $A_0=\varnothing$ and the [half-plane-capacity parameterization](../../../../../../half-plane-capacity-parameterization.md) $\operatorname{hcap}(A_t)=2t$. The [Conformal Markov property of SLE](../../../../../../conformal-markov-property-of-sle.md) combines invariance under conformal changes of the marked domain with restarting after an initial hull has been removed.

In the half-plane this means, first, that $(r^{-1}A_{r^2t})_{t\geq0}$ has the same law as $(A_t)_{t\geq0}$ for every $r>0$. Second, conditionally on $\mathcal F_t$, the future hulls mapped by $g_t-U_t$,

$$
\widehat A_s=(g_t-U_t)(A_{t+s}\setminus A_t),\qquad s\geq0,
$$

with the usual hull closure, have the original law and are independent of $\mathcal F_t$. Their capacity is $2s$ by the [half-plane-capacity composition rule](../../../../../../half-plane-capacity-composition-rule.md). One may require the same restarting property at finite [stopping times](../../../../../../stopping-time.md).

Equivalently, the driver has the scaling law and conditional increment law

$$
\boxed{(r^{-1}U_{r^2s})_{s\geq0}\overset{d}=(U_s)_{s\geq0},\qquad
(U_{t+s}-U_t)_{s\geq0}\mid\mathcal F_t\ \overset{d}=(U_s)_{s\geq0}\text{ independently}.}
$$

The conformal invariance clause matters: the restarting property alone would also allow a Brownian driver with deterministic drift.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

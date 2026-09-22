<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The indexing defect also affects the downstream claim. For the two inputs in part (b), now choose $\lambda<d<c$. The constant input has zero downstream [queue workload](../../../../../../workload-of-a-queue.md), while the input with $a_0=c+1$ has

$$
Q_0(b,d)=c+1-d,\qquad Q_0(b,c)=1,\qquad R_0(b,c,d)=c-d>0.
$$

Their printed distance is zero, so the literal post-slot downstream [continuity](../../../../../../continuous-function.md) assertion is false as well.

In the corrected [weighted cumulative-input topology for a slotted queue](../../../../../../weighted-cumulative-input-topology-for-a-slotted-queue.md), apply the finite-window proof of part (b) separately with services $d$ and $c$. Both have strictly negative long-window drift because $\lambda<d<c$. There are a neighborhood of $a$ and finite constants $C_d,C_c$ such that

$$
|R_0(a,c,d)-R_0(b,c,d)|
\leq |Q_0(a,d)-Q_0(b,d)|+|Q_0(a,c)-Q_0(b,c)|
\leq(C_d+C_c)d_\#(a,b).
$$

This proves [continuity](../../../../../../continuous-function.md), and indeed local [Lipschitz continuity](../../../../../../lipschitz-continuity.md), for the intended downstream function.

Suppose a family of random arrival paths $a^{(L)}$ has a [large deviation principle](../../../../../../large-deviation-principle.md) in this corrected input space, at speed $L$ with [good rate function](../../../../../../good-rate-function.md) $\mathcal I$. The [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) then gives the downstream [good rate function](../../../../../../good-rate-function.md)

$$
\boxed{J_R(r)=\inf\{\mathcal I(a):Q_0(a,d)-Q_0(a,c)=r\}.}
$$

It is infinity for $r<0$. The path [large deviation principle](../../../../../../large-deviation-principle.md), its topology, and its subcritical domain must actually be established for the chosen stochastic model: a collection of finite-dimensional [large deviation principles](../../../../../../large-deviation-principle.md) alone does not control infinitely long workload windows. Nor should upstream departures be assumed [independent](../../../../../../independent-random-variables.md); the path contraction avoids that unjustified assumption.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Every function $h$ with [Lipschitz constant](../../../../../../lipschitz-constant.md) at most $1$ yields a feasible pair $(h,-h)$, and replacing $h$ by $-h$ reverses the objective. Hence

$$
\gamma(P,Q)=\sup_{\|h\|_L\leq1}\left(\int h\,dP-\int h\,dQ\right)\leq m_L(P,Q).
$$

Conversely, the [Lipschitz regularization of transport potentials](../../../../../../lipschitz-regularization-of-transport-potentials.md) in part iii dominates every feasible pair by $(h,-h)$ with $\|h\|_L\leq1$, so $m_L\leq\gamma$. Together with the preceding parts this proves the [Kantorovich–Rubinstein theorem](../../../../../../kantorovich-rubinstein-theorem.md) here in all four requested forms:

$$
\boxed{m_d(P,Q)=W(P,Q)=m_L(P,Q)=\gamma(P,Q)}.
$$

The seminorm convention is essential. If instead $\|h\|_L$ meant $\|h\|_\infty+\operatorname{Lip}(h)$, the equality would fail: on a two-point space at distance $2$, with point masses at the two different points, $W=2$ whereas the latter unit-ball supremum is $1$. Indeed, an oscillation $a$ needs supremum [norm](../../../../../../norm.md) at least $a/2$ and [Lipschitz constant](../../../../../../lipschitz-constant.md) $a/2$, so the sum [norm](../../../../../../norm.md) bounds $a$ by $1$, attained by values $-1/2,1/2$. This distinguishes the [Lipschitz](../../../../../../lipschitz-continuity.md) seminorm used above from a full bounded-[Lipschitz](../../../../../../lipschitz-continuity.md) [norm](../../../../../../norm.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

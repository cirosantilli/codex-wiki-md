<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [dyadic slope martingale](../../../../../../dyadic-slope-martingale.md) is uniformly bounded by $L$. The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives an almost-sure limit $\dot f$, and [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives [L1 convergence](../../../../../../convergence-in-l1.md). Define $\dot f=0$ on the null exceptional set and at the endpoint. This gives a [measurable](../../../../../../measurability.md) representative with $|\dot f|\leq L$ everywhere.

If $a,b$ are [dyadic rationals](../../../../../../dyadic-rational.md), then for every sufficiently fine grid the integral telescopes:

$$
\int_a^b X_n(x)\,dx=\sum_{[u,v)\subset[a,b)}\bigl(f(v)-f(u)\bigr)=f(b)-f(a).
$$

Pass to the limit by [L1 convergence](../../../../../../convergence-in-l1.md). For arbitrary endpoints choose dyadic $a_j\to a$, $b_j\to b$ with $a_j\leq b_j$. The error in the integrals is at most $L(|a_j-a|+|b_j-b|)$, and [Lipschitz continuity](../../../../../../lipschitz-continuity.md) controls the error in the endpoint values by the same expression. Therefore

$$
\boxed{\int_a^b\dot f(x)\,dx=f(b)-f(a)\quad(0\leq a\leq b\leq1),\qquad\|\dot f\|_\infty\leq L.}
$$

This constructs the bounded integral density directly, without assuming in advance that a [Lipschitz function](../../../../../../lipschitz-continuity.md) has an [almost everywhere](../../../../../../almost-everywhere.md) derivative.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

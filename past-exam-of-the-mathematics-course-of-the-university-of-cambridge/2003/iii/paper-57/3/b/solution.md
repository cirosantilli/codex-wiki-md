<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the graph embedding $\iota(q)=(q,p(q))$, pull back the [symplectic form](../../../../../../symplectic-form.md) in [Darboux coordinates](../../../../../../darboux-chart.md):

$$
\iota^*\omega=\sum_{i,j}\frac{\partial p_i}{\partial q^j}\,dq^i\wedge dq^j
=\sum_{i<j}\left(\frac{\partial p_i}{\partial q^j}-\frac{\partial p_j}{\partial q^i}\right)dq^i\wedge dq^j.
$$

The coordinate two-forms are linearly independent. The graph has dimension $n$, so it is a [Lagrangian submanifold](../../../../../../lagrangian-submanifold.md) exactly when this [pullback](../../../../../../pullback-category-theory.md) vanishes, equivalently when its displayed coefficient matrix is symmetric.

Let $\theta_L=\sum_i p_i(q)dq^i$. Then $d\theta_L=-\iota^*\omega$, so the same condition says that $\theta_L$ is a [closed differential form](../../../../../../closed-differential-form.md). On a sufficiently small contractible coordinate neighborhood the [Poincaré lemma](../../../../../../poincare-lemma.md) supplies $S$ with $\theta_L=dS$. Consequently

$$
\boxed{p_i=\partial_iS.}
$$

One explicit primitive on a star-shaped neighborhood of $q_0$ is $S(q)=S(q_0)+\int_0^1p_i(q_0+t(q-q_0))(q^i-q_0^i)\,dt$. Differentiate it and use $\partial_jp_i=\partial_ip_j$ to recognize the derivative of $t p_j(q_0+t(q-q_0))$; the result is $\partial_jS=p_j(q)$. Conversely $p=dS$ has symmetric mixed derivatives and gives a [Lagrangian graph](../../../../../../lagrangian-graph.md). This construction requires the local projection to the $q$ coordinates to be nonsingular. A general [Lagrangian submanifold](../../../../../../lagrangian-submanifold.md) need not be such a graph in a preassigned chart, and a closed one-form on a larger domain need not be globally exact.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

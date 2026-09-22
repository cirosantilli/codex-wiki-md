<h1 id="15b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a regular [Lagrangian](../../../../../../lagrangian.md), define the [canonical momentum](../../../../../../canonical-momentum.md) $p_i=\partial L/\partial\dot q_i$ and invert this relation for $\dot q(q,p,t)$. Its [Legendre transform](../../../../../../convex-conjugate.md) is the [Hamiltonian](../../../../../../hamiltonian.md)

$$
H(q,p,t)=p\mathbin\cdot\dot q-L(q,\dot q,t).
$$

Since $L\,dt=p\cdot dq-H\,dt$, the [action](../../../../../../action.md) is

$$
S=\int_{t_1}^{t_2}(p\cdot\dot q-H)\,dt
=\int(p\cdot dq-H\,dt).
$$

For independent variations with $\delta q(t_1)=\delta q(t_2)=0$,

$$
\delta S=\int_{t_1}^{t_2}
\left[(\dot q-\partial_pH)\cdot\delta p
-(\dot p+\partial_qH)\cdot\delta q\right]dt.
$$

Stationarity for arbitrary $\delta p$ and $\delta q$ gives [Hamilton's equations](../../../../../../hamilton-s-equations.md) $\dot q=\partial_pH$ and $\dot p=-\partial_qH$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15B](../../15b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

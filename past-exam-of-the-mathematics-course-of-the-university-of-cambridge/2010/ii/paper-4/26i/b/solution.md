<h1 id="26i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this [linear birth process with catastrophes](../../../../../../linear-birth-process-with-catastrophes.md), the off-diagonal entries of the [Q-matrix](../../../../../../transition-rate-matrix.md) are

$$
q_{0,1}=\lambda,\qquad
q_{n,n+1}=\lambda(n+1),\qquad q_{n,0}=\mu\quad(n\ge1),
$$

with all other off-diagonal entries zero. The diagonal entries are $q_{00}=-\lambda$ and $q_{nn}=-[\lambda(n+1)+\mu]$ for $n\ge1$. At zero there is no separate catastrophe transition, because it would not change the state.

The chain is irreducible: every positive state can jump to zero, and from zero any finite sequence of births has positive probability. To prove nonexplosion, couple it with the [linear birth process with immigration](../../../../../../linear-birth-process-with-immigration.md) having birth rate $\lambda(n+1)$ and no catastrophes. Its mean population is finite at each finite time, obtained from $m'=\lambda(m+1)$, or its exponential holding-time sum diverges since $\sum_n1/[\lambda(n+1)]=\infty$. Couple births monotonically and implement catastrophes with an independent rate-$\mu$ Poisson clock, resetting the smaller population. On a finite time interval the dominating pure-birth process has finitely many births, and the catastrophe clock finitely many rings. Thus the original chain is nonexplosive.

For its [jump chain](../../../../../../jump-chain.md), the transitions are

$$
\boxed{P_{0,1}=1,\quad
P_{n,n+1}=\frac{\lambda(n+1)}{\lambda(n+1)+\mu},\quad
P_{n,0}=\frac{\mu}{\lambda(n+1)+\mu}\quad(n\ge1).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

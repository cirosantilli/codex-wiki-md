<h1 id="21h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a [matrix game](../../../../../../matrix-game.md), entry $a_{ij}$ is the row player's payoff, and the column player's payoff is $-a_{ij}$. A [mixed strategy](../../../../../../mixed-strategy.md) is a probability vector over the available rows or columns. With strategies $p,q$, the row payoff is $p^TAq$. Its [optimal mixed strategy](../../../../../../optimal-mixed-strategy.md) maximizes its guaranteed payoff, while the column player minimizes the largest row payoff:

$$
\boxed{\max_{p\in\Delta_m}\min_{q\in\Delta_n}p^TAq
=\min_{q\in\Delta_n}\max_{p\in\Delta_m}p^TAq=v.}
$$

The equality is the finite [minimax theorem](../../../../../../minimax-theorem.md). Equivalently the row player maximizes $\min_j(p^TA)_j$, and the column player minimizes $\max_i(Aq)_i$. Each optimal strategy guarantees its corresponding bound against every opponent strategy; for the column player's own negative payoff this is also a maximin strategy.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

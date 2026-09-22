<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

Let $(q_R,q_S,q_P)$ be player two's [mixed strategy](../../../../../mixed-strategy.md) in [Rock paper scissors](../../../../../rock-paper-scissors.md). The respective expected payoffs from choosing rock, scissors and paper are $1-p$, $-p$ and $2p-1$. Thus player two solves the [linear programming](../../../../../linear-programming.md) problem

$$
\max\ (1-p)q_R-pq_S+(2p-1)q_P,
\qquad q_R,q_S,q_P\ge0,\quad q_R+q_S+q_P=1.
$$

A linear objective on this probability simplex is maximized by a largest-payoff pure response, or by any mixture of tied maximizers. Scissors is never a maximizing response: rock exceeds it by one. Comparing the other two gives $1-p\gtreqless2p-1$ according as $p\lesseqgtr2/3$. Therefore

$$
\boxed{\begin{cases}
(q_R,q_S,q_P)=(1,0,0),&p<2/3,\\
(q_R,q_S,q_P)=(q,0,1-q),\ 0\le q\le1,&p=2/3,\\
(q_R,q_S,q_P)=(0,0,1),&p>2/3.
\end{cases}}
$$

The optimal expected payoff is $1-p$ below the tie and $2p-1$ above it, with value $1/3$ at the tie.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

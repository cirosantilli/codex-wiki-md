<h1 id="m/m1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First the entries must be nonnegative: together with the given $a,b\geq0$, validity of the [transition matrix](../../../../../../stochastic-matrix.md) requires $0\leq a\leq1$ and $0\leq b\leq1/3$. Every row then sums to one.

The only incoming edge to state $2$ is $1\to2$, of [probability](../../../../../../probability.md) $a$. If $a=0$, no other state can reach $2$, so the chain is not irreducible. If $a>0$, all edges in the directed cycle

$$
1\longrightarrow2\longrightarrow3\longrightarrow4\longrightarrow1
$$

have positive [probability](../../../../../../probability.md), since $P_{23}=1/3+b>0$, $P_{34}=1$ and $P_{41}=1/2$. Traversing this cycle connects every state to every other state. Therefore

$$
\boxed{\text{Irreducible exactly when }0<a\leq1,\quad0\leq b\leq\frac13.}
$$

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [M1](../../../m1.md)
4. [M](../../../../m.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

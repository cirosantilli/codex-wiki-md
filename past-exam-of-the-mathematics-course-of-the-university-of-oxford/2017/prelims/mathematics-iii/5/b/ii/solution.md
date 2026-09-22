<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $q_n=\mathbb P(M_n=Y)$. The [law of total probability](../../../../../../../law-of-total-probability.md) applied to the current [markov chain state](../../../../../../../markov-chain-state.md) gives

$$
p_n=\frac12p_{n-1}+\frac38q_{n-1},\qquad q_{n-1}=\frac12p_{n-2}\quad(n\ge2).
$$

The second equality holds because $Y$ can only be reached from $X$. Eliminating $q_{n-1}$ gives the [linear recurrence relation](../../../../../../../linear-recurrence-relation.md)

$$
\boxed{16p_n=8p_{n-1}+3p_{n-2},\qquad n\ge2.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

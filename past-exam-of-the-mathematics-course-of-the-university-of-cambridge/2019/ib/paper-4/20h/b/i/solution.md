<h1 id="20h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Starting from zero, one valid run of the [Ford-Fulkerson algorithm](../../../../../../../ford-fulkerson-algorithm.md) augments along

$$
\begin{aligned}
S\to a\to d\to T &\quad\text{by }1,\\
S\to b\to d\to T &\quad\text{by }2,\\
S\to b\to e\to T &\quad\text{by }1,\\
S\to c\to e\to T &\quad\text{by }4.
\end{aligned}
$$

The resulting nonzero edge flows are

$$
\begin{array}{c|ccccccccc}
\text{edge}&Sa&Sb&Sc&ad&bd&be&ce&dT&eT\\ \hline
\text{flow}&1&3&4&1&2&1&4&3&5
\end{array}
$$

and they obey every [capacity constraint](../../../../../../../capacity-constraint.md) and every flow-conservation equation. The flow value is

$$
\boxed{|f|=1+3+4=8}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [20H](../../../20h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write each [Horn clause](../../../../../../horn-clause.md) as an implication

$$
x_1\wedge\cdots\wedge x_k\longrightarrow y
$$

when it has one positive literal $y$, or as a forbidden conjunction

$$
\neg(x_1\wedge\cdots\wedge x_k)
$$

when it has none. Start with every variable false. Repeatedly, whenever all antecedents of an implication are true, set its conclusion true. If a forbidden conjunction ever has all antecedents true, report unsatisfiable; otherwise stop when no change is possible and return the resulting assignment.

Each step changes a previously false variable to true, so at most the number of variables steps occur; scanning all clauses after each step is polynomial time. For correctness, every satisfying assignment must set every variable derived by this [Horn-SAT forward-chaining algorithm](../../../../../../horn-sat-forward-chaining-algorithm.md) to true, by induction over the derivation. Therefore, if the algorithm violates a negative clause, every assignment violates it. If no violation occurs, all implications and all negative clauses are satisfied by the final assignment. This proves polynomial-time decidability.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

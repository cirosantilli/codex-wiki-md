<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [serial database schedule](../../../../../serial-database-schedule.md) is obtained by running the three [database transactions](../../../../../database-transaction.md) in the order $T_1,T_2,T_3$:

$$
\boxed{W_1(A),R_1(B),W_1(C),\ W_2(A),W_2(C),R_2(B),\ R_3(B),R_3(A),R_3(D).}
$$

A genuinely interleaved [conflict-serializable database schedule](../../../../../conflict-serializable-database-schedule.md) with the same serial order is

$$
\boxed{W_1(A),R_3(B),R_1(B),W_1(C),W_2(A),W_2(C),R_2(B),R_3(A),R_3(D).}
$$

The early $R_3(B)$ conflicts with nothing: all accesses to $B$ are reads. The conflicts on $A$ give edges $T_1\to T_2$, $T_1\to T_3$ and $T_2\to T_3$ in the [database precedence graph](../../../../../database-precedence-graph.md), while the writes to $C$ give the already present edge $T_1\to T_2$. This [database precedence graph](../../../../../database-precedence-graph.md) has no directed cycle and admits the order $T_1,T_2,T_3$. Moving the early $R_3(B)$ after $R_2(B)$ swaps it only past non-conflicting operations, recovering the displayed [serial database schedule](../../../../../serial-database-schedule.md).

For a [database schedule](../../../../../database-schedule.md) that is not a [conflict-serializable database schedule](../../../../../conflict-serializable-database-schedule.md), take

$$
\boxed{W_1(A),W_2(A),W_2(C),R_1(B),W_1(C),R_2(B),R_3(B),R_3(A),R_3(D).}
$$

On $A$, $W_1(A)$ before $W_2(A)$ forces $T_1\to T_2$. On $C$, $W_2(C)$ before $W_1(C)$ forces $T_2\to T_1$. The resulting directed cycle prevents any serial ordering from preserving all conflicts. Each of the three displayed [database schedules](../../../../../database-schedule.md) preserves the operation order inside every [database transaction](../../../../../database-transaction.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

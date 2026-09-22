<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $0$ and $1$ for false and true [truth values](../../../../../truth-value.md). The [truth table](../../../../../truth-table.md) is:

| $A$ | $B$ | $C$ | $A\leftrightarrow B$ | $\neg B\to C$ | $\varphi$ |
| --- | --- | --- | --- | --- | --- |
| $0$ | $0$ | $0$ | $1$ | $0$ | $0$ |
| $0$ | $0$ | $1$ | $1$ | $1$ | $1$ |
| $0$ | $1$ | $0$ | $0$ | $1$ | $0$ |
| $0$ | $1$ | $1$ | $0$ | $1$ | $0$ |
| $1$ | $0$ | $0$ | $0$ | $0$ | $0$ |
| $1$ | $0$ | $1$ | $0$ | $1$ | $0$ |
| $1$ | $1$ | $0$ | $1$ | $1$ | $1$ |
| $1$ | $1$ | $1$ | $1$ | $1$ | $1$ |

The two satisfying rows with $A=B=1$ combine by eliminating $C$, while the remaining satisfying row has $A=B=0,C=1$. An equivalent [disjunctive normal form](../../../../../disjunctive-normal-form.md) is therefore

$$
\boxed{(A\land B)\lor(\neg A\land\neg B\land C).}
$$

Expanding the [logical biconditional](../../../../../logical-biconditional.md) into its two implications, and using $\neg B\to C\equiv B\lor C$, gives the [conjunctive normal form](../../../../../conjunctive-normal-form.md)

$$
\boxed{(\neg A\lor B)\land(A\lor\neg B)\land(B\lor C).}
$$

Each form has exactly the same three [satisfying assignments](../../../../../satisfying-assignment.md) as the original [propositional formula](../../../../../propositional-formula.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Introduction to formal proof](../../introduction-to-formal-proof.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\tau$ for the table. The positive initial [planning fluents](../../../../../planning-fluent.md) read from the original figure are

$$
\boxed{I=\{\operatorname{On}(A,\tau),\operatorname{On}(B,\tau),\operatorname{On}(C,A),\operatorname{Clear}(B),\operatorname{Clear}(C)\}.}
$$

The static type facts are $\operatorname{Block}(A)$, $\operatorname{Block}(B)$ and $\operatorname{Block}(C)$; the table is not a block. With an explicit table-availability [predicate](../../../../../predicate.md), take $\operatorname{Clear}(\tau)$ to be permanently true. Under the [closed-world assumption](../../../../../closed-world-assumption.md), all other well-typed initial [planning fluents](../../../../../planning-fluent.md) are false; in particular, $A$ is not clear.

The goal is the partial-state [conjunction](../../../../../conjunction-astronomy.md)

$$
\boxed{G=\operatorname{On}(A,B)\land\operatorname{On}(B,C).}
$$

It need not redundantly prescribe every final fact. With only these three blocks and a valid [blocks world](../../../../../blocks-world.md) state, the completed stack also places $C$ on the table and leaves $A$ clear.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

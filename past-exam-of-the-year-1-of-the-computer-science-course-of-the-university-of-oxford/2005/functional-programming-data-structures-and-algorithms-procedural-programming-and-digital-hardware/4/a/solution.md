<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) splits an instance into smaller instances of the same kind, solves them recursively, and combines their answers. The smaller instances should be sufficiently smaller to ensure [algorithm termination](../../../../../algorithm-termination.md); the combination cost determines whether splitting saves work. The two halves of [merge sort](../../../../../merge-sort.md) illustrate this separation.

[Dynamic programming](../../../../../dynamic-programming.md) identifies a collection of subproblems and dependencies among them, solves each distinct subproblem once, and stores its answer. A table in dependency order or [memoization](../../../../../memoization.md) prevents repeated evaluation of overlapping subproblems. For optimization, an [optimal substructure](../../../../../optimal-substructure.md) argument justifies constructing an optimal answer from optimal smaller answers.

A [greedy algorithm](../../../../../greedy-algorithm.md) repeatedly makes a locally best feasible choice and commits to it. It avoids exploring alternative continuations. [Algorithm correctness](../../../../../algorithm-correctness.md) therefore needs a [greedy-choice property](../../../../../greedy-choice-property.md), often proved by replacing the first choice of an optimal solution with the greedy choice without worsening it.

$$
\boxed{\text{divide and combine; reuse subproblem answers; commit to safe local choices}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

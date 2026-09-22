<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the [coin change problem](../../../../../coin-change-problem.md), take denominations $\{1,3,4\}$ and target amount $6$. The natural [greedy algorithm](../../../../../greedy-algorithm.md) repeatedly chooses the largest denomination not exceeding the remaining amount. It chooses $4$, then $1$, then $1$, for three coins. Yet $3+3=6$ uses only two.

Two is optimal: one coin cannot make $6$ because denomination $6$ is absent, and the displayed pair attains the lower bound. Therefore

$$
\boxed{\text{greedy: }4+1+1\ (3\text{ coins});\qquad
\text{optimal: }3+3\ (2\text{ coins}).}
$$

The locally largest first coin loses the possibility of using the better pair of threes. This supplies a concrete failure of the [greedy-choice property](../../../../../greedy-choice-property.md); [optimal substructure](../../../../../optimal-substructure.md) alone does not justify the greedy choice. The [dynamic programming](../../../../../dynamic-programming.md) recurrence from part (b) would compare all feasible first or last denominations and find the pair.

## ↑ Ancestors (12)

1. [C](../c.md)
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

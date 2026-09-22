<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dynamic programming](../../../../../dynamic-programming.md) stores answers to overlapping subproblems so they can be reused. Its [optimal substructure](../../../../../optimal-substructure.md) requirement, the principle of optimality, says that an optimal answer's remaining subproblem solution must itself be optimal once the final decision and state are fixed.

For [global sequence alignment without mismatches](../../../../../global-sequence-alignment-without-mismatches.md), use the two prefix lengths as the state. A final column is either a letter of the first string opposite a gap, a gap opposite a letter of the second, or two equal letters. Removing that column leaves one of three smaller prefix problems. If its alignment were suboptimal, replacing it by a better alignment would improve the whole answer. Many different alignments reach the same prefix state, making reuse valuable. Unequal-letter columns and double-gap columns are forbidden, rather than assigned ordinary finite penalties.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="s/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start the augmenting-path algorithm from the zero flow. With integer capacities and an integer [electric current](../../../../../electric-current.md) flow, every residual capacity is an integer, so a path bottleneck is a positive integer. Augmenting by it preserves integrality and increases the flow value by at least one. The value is bounded by the finite total capacity leaving the source, so the process terminates. At termination there is no [augmenting path](../../../../../augmenting-path.md), hence the flow is maximum by the [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md). Its value is an integer.

Equivalently a minimum cut has capacity equal to the sum of integer arc capacities, so the [maximum flow](../../../../../maximum-flow-problem.md) value equals an integer. Thus **integer capacities guarantee an integer optimal volume**, even though arbitrary feasible real-valued flows need not themselves have integer entries.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [S](../../../s.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A length-zero [graph path](../../../../../path-in-a-graph.md) starts and ends at the same [vertex](../../../../../vertex-graph-theory.md). Therefore $P_0$ is the [Boolean](../../../../../boolean-data-type.md) [identity matrix](../../../../../identity-matrix.md). A [graph path](../../../../../path-in-a-graph.md) of length at most one is either such a stationary [graph path](../../../../../path-in-a-graph.md) or one original directed [edge](../../../../../edge-of-a-graph.md):

$$
\boxed{P_0[i,j]=(i=j),\qquad P_1[i,j]=(i=j)\lor E[i,j],\qquad P_1=I\lor E.}
$$

The logical disjunction is entrywise. Diagonal entries of $E$ may be false if there are no [self-loops](../../../../../loop-graph-theory.md), but every diagonal entry of $P_1$ is true because the zero-length [graph path](../../../../../path-in-a-graph.md) is allowed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

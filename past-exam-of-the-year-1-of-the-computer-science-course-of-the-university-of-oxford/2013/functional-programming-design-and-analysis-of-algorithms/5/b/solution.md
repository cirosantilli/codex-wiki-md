<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [graph path](../../../../../path-in-a-graph.md) of length at most $k+1$ either already has length at most $k$, or consists of a prefix of length at most $k$ followed by one [edge](../../../../../edge-of-a-graph.md). Therefore

$$
\boxed{P_{k+1}[i,j]=P_k[i,j]\lor\bigvee_{t=0}^{n-1}\bigl(P_k[i,t]\land E[t,j]\bigr).}
$$

The forward implication follows by removing the final [edge](../../../../../edge-of-a-graph.md) of a nonempty [graph path](../../../../../path-in-a-graph.md). Conversely, concatenating the indicated prefix and [edge](../../../../../edge-of-a-graph.md) gives a [walk](../../../../../walk-in-a-graph.md) of length at most $k+1$, and removing repetitions if necessary gives a [graph path](../../../../../path-in-a-graph.md) no longer than that [walk](../../../../../walk-in-a-graph.md).

Writing $\odot$ for [Boolean matrix multiplication](../../../../../boolean-matrix-multiplication.md), the formula is $P_{k+1}=P_k\lor(P_k\odot E)$. Because $P_1$ includes the [identity matrix](../../../../../identity-matrix.md), an equivalent formula is

$$
\boxed{P_{k+1}=P_k\odot P_1.}
$$

Compute each new [matrix](../../../../../matrix.md) from an unchanged copy of the preceding [matrix](../../../../../matrix.md), so the subscript continues to specify exactly the length bound.

## ↑ Ancestors (12)

1. [B](../b.md)
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

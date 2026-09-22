<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The cost is **$\Theta(n)$ arithmetic and comparison operations** under shared [lazy evaluation](../../../../../lazy-evaluation.md) and unit-cost operations on the numeric values. There are only three mapped streams and two merge nodes. Before the first $n$ output cells are produced, each node advances at most $n+O(1)$ input positions; each advance does a bounded number of operations. Producing the $n$ output cells also gives an $\Omega(n)$ lower bound.

This is [stream sharing in Hamming-number construction](../../../../../stream-sharing-in-hamming-number-construction.md). It relies on sharing the recursive list cells, and is not a bound on bit operations: multiplying or comparing arbitrarily large `Integer` values costs more as their representations grow.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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

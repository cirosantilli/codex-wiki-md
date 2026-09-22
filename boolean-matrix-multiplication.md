# Boolean matrix multiplication

↑ **Parent:** [Matrix multiplication](matrix-multiplication.md)

For [Boolean](boolean-data-type.md) [matrices](matrix.md), replace numerical [addition](addition.md) by logical disjunction and [multiplication](multiplication.md) by logical conjunction. Applied to [adjacency matrices](adjacency-matrix.md), the product records a [walk](walk-in-a-graph.md) formed by following one segment represented by the first [matrix](matrix.md) and one represented by the second. For an [adjacency matrix](adjacency-matrix.md) $A$ on $n\geq1$ [vertices](vertex-graph-theory.md), start from $I\lor A$. Repeated squaring then computes [reflexive transitive closure](reflexive-transitive-closure.md) once the exponent reaches $n-1$: the identity entries pad shorter [walks](walk-in-a-graph.md), and every reachable pair has a [simple path](path-in-a-graph.md) of length at most $n-1$.

## ↑ Ancestors (9)

1. [Matrix multiplication](matrix-multiplication.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/5/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/5/e/solution.md)

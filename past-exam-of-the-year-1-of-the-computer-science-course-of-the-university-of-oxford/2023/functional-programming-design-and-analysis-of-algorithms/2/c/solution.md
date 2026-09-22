<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The most informative [occurrence-position representation of a sequence](../../../../../occurrence-position-representation-of-a-sequence.md) of natural numbers is
```
naturals :: Seq Integer
naturals v
  | v < 0 = []
  | otherwise = [v]
```
Each nonnegative integer occurs once at its own index, and negative integers never occur.

**This is not equal to `rep [0..]` under [lazy evaluation](../../../../../lazy-evaluation.md).** For a nonnegative query `v`, `rep` eventually emits `v`, but then searches forever for another occurrence: its result has the shape `v : undefined`, rather than the terminating singleton `[v]`. For a negative query, even the outer constructor is never produced, whereas `naturals` immediately returns `[]`.

No general, correct `rep :: Eq a => [a] -> Seq a` can always certify those absences from an arbitrary infinite input. A terminating certification has inspected only finitely many elements, and the same prefix could be followed by the supposedly absent value, or by a further occurrence of it. Extra knowledge changes the problem: for a promised strictly increasing integer input, a search can stop with `[]` when it first exceeds the query and return `[i]` immediately upon equality. That specialised representation can produce `naturals`; a generic search cannot. This is the [absence-detection obstruction for infinite lists](../../../../../absence-detection-obstruction-for-infinite-lists.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

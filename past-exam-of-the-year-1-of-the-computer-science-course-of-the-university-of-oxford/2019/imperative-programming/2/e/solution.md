<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Test singleton and two-element segments, first/last/interior requested ranks, nonzero segment offsets, already sorted and reversed inputs, random inputs, all-equal inputs and several patterns of duplicates. Include `Int.MinValue` and `Int.MaxValue` to expose overflow-prone comparisons. An independent sorted copy supplies the value oracle; also check preservation of the segment's [multiset](../../../../../multiset.md) and of all outside entries. For speed tests, increase segment size and include deliberately unfavorable pivot arrangements, rather than timing random inputs alone.

**Distinct entries do not guarantee linear worst-case time: the worst case is $\Theta(N^2)$.** A median of three can repeatedly be the second-smallest remaining value, leaving a segment of size $N-2$ when seeking its maximum. The [quadratic median-of-three selection family](../../../../../quadratic-median-of-three-selection-family.md) gives explicit distinct inputs realizing this behavior for the implementation above; one six-entry member is $[1,4,3,0,2,5]$. Its recurrence is $T(N)=T(N-2)+\Theta(N)$, yielding a quadratic sum. Balanced reductions instead give $T(N)=T(N/2)+\Theta(N)=\Theta(N)$. Randomized or suitable average-case analyses give expected linear selection, but this deterministic heuristic alone supplies no such worst-case guarantee. Unlike [Quicksort](../../../../../quicksort.md), [Quickselect](../../../../../quickselect.md) explores only one side, so a balanced run is linear rather than $\Theta(N\log N)$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

A compatible `Ord` instance supplies a [total order](../../../../../total-order.md), so use [comparison sort](../../../../../comparison-sort.md) to put equal values together in $O(n\log n)$ time and then group adjacent equals in [linear time](../../../../../linear-time.md). To preserve the first-occurrence group ordering of part (f), first tag every element with its original index and [stable sorting](../../../../../stable-sorting.md) by value. Group the sorted records by value; stability preserves their internal input order. Each group's first record carries its smallest original index. Sort the groups by that index and finally remove the tags. The second sort has at most $n$ records, so the total remains **$O(n\log n)$ time** and $O(n)$ storage. Merely returning the value-sorted groups could reorder the classes, so the index step matters when preserving the exact earlier convention. The stronger interface evades the equality-only lower bound by permitting order comparisons.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

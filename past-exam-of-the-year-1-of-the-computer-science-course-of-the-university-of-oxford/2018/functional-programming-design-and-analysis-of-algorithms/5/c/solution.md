<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Sort records `(value,original_index)` by value using [merge sort](../../../../../merge-sort.md). For each record with value $a$, run [binary search](../../../../../binary-search.md) for value $2a$ among the sorted records; return the two retained original indices at the first match, otherwise return `nil` after all records.

If a valid pair exists, its smaller entry is inspected and the matching doubled entry is found by [binary search](../../../../../binary-search.md). Conversely every returned pair satisfies the requested equality. Positivity gives $2a>a$, so the returned entries are distinct even if other entries repeat. Sorting costs $O(n\log n)$, and at most $n$ [binary searches](../../../../../binary-search.md) cost $O(n\log n)$ altogether. **Total time is $O(n\log n)$**, using the paper's unit-cost arithmetic model; doubling large machine integers would require overflow-safe arithmetic.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

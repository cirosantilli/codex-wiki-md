<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Arrange that each state already begins with the next passing element, or is empty:

```
filter p = unfold null head next . seek
  where
    seek = dropWhile (not . p)
    next = seek . tail
```

The initial `seek` skips the rejected prefix. After an element is emitted, `next` removes it and skips the following rejected run. Thus `null` guards both partial list operations and the [filtering a list by unfolding](../../../../../filtering-a-list-by-unfolding.md) invariant is preserved.

For a finite input of length $n$ and constant-cost predicate evaluation, each input element is tested once and each list cell is passed a bounded number of times: the total work is **$O(n)$**, as for the usual recursive [list filter](../../../../../list-filter.md). This version may have different constant overhead. Recomputing `dropWhile` independently in the stopping, output and transition expressions could repeat scans; keeping the already-filtered suffix as state avoids that. On an infinite rejected tail, finding another output diverges, just as the standard lazy filter does.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using the specified [list unfold](../../../../../list-unfold.md), the definitions are

```
map f     = unfold null (f . head) tail
iterate f = unfold (const False) id f
```

For `map`, the current state is the remaining input list. `null` prevents `head` and `tail` from being evaluated on an empty list. For `iterate`, the stop predicate is always false and the output is the current state itself. Its transition is `f`, so the original seed is emitted before the first application of `f`.

## ↑ Ancestors (12)

1. [D](../d.md)
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

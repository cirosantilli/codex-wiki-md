<h1 id="5/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep each weight attached to its value while sorting, then return the first cumulative weight reaching one half:

```
weightedMedian(A, weights):
    R = records (A[i], weights[i], i), sorted by first component
    cumulative = 0
    for (value, weight, original_index) in R:
        cumulative = cumulative + weight
        if cumulative >= 1/2:
            return original_index
```

All weights are positive, so the cumulative weights strictly increase. At the returned entry the mass strictly to its left is below one half, while the mass strictly to its right is at most one half. This is the **[lower weighted median](../../../../../../lower-weighted-median.md)**, including the exact equality case: stop at the earlier value whose cumulative mass is exactly one half. Sorting takes $O(n\log n)$ and the scan takes $O(n)$, giving **$O(n\log n)$ time**.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

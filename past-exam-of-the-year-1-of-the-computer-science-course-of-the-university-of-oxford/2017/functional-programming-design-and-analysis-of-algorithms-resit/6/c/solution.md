<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $e_i$ be the best sum of a segment ending at position $i$, allowing the empty segment with sum zero. The [maximum subarray problem](../../../../../maximum-subarray-problem.md) recurrence is

$$
\boxed{e_0=0,\qquad e_i=\max(0,e_{i-1}+a_i),\qquad B_i=\max(B_{i-1},e_i),\ B_0=0.}
$$

An optimal nonempty segment ending at $i$ extends the best suffix ending at $i-1$, or starts fresh; a negative suffix cannot help. Keep its start index and record endpoints whenever a new overall best is found:

```
suffix = 0; best = 0
start = 0; bestLeft = 0; bestRight = 0
for i = 0,...,n-1:
    suffix = suffix + A[i]
    if suffix < 0:
        suffix = 0; start = i+1
    if suffix > best:
        best = suffix
        bestLeft = start; bestRight = i+1
return A[bestLeft:bestRight]
```

The half-open endpoint interval is empty initially, so empty input and all-negative input correctly return an empty segment. The invariant identifies the best nonnegative suffix and the best segment in the scanned prefix, proving correctness. This is [Kadane's algorithm](../../../../../kadane-s-algorithm.md), using **$O(n)$ time and $O(1)$ auxiliary space**, excluding the returned slice. The displayed example yields **sum $55$**, from the segment $10,-5,40,10$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
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

<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [minimum search in a rotated distinct array](../../../../../minimum-search-in-a-rotated-distinct-array.md), then return the cyclic predecessor of the minimum:

```
rotatedMaximum(A):
    n = length(A)                 # require n >= 1
    lo = 0
    hi = n - 1
    while lo < hi:
        mid = floor((lo + hi) / 2)
        if A[mid] > A[hi]:
            lo = mid + 1
        else:
            hi = mid
    return A[(lo + n - 1) mod n]
```

The [loop invariant](../../../../../loop-invariant.md) says that the minimum index lies in the inclusive interval. If `A[mid] > A[hi]`, the rotation break lies to the right of `mid`; otherwise the segment from `mid` to `hi` is increasing and its indices after `mid` cannot be the minimum. Each update at least halves the interval. Distinct entries make the comparison decisive, including a completely unshifted array. The predecessor of the unique minimum is the maximum, and the one-element case returns that element. The running time is **$O(\log n)$**, with $O(1)$ auxiliary space.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
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

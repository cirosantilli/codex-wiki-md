<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Save the root, move the last active entry to the root, shrink the active prefix, then restore [heap order](../../../../../heap-order.md) by [heapify down](../../../../../sift-down.md):
```
ExtractMin(A):
    if A.heap_size == 0:
        error "empty heap"
    answer = A[0]
    A[0] = A[A.heap_size-1]
    A.heap_size = A.heap_size-1
    if A.heap_size > 0:
        SiftDown(A,0)
    return answer

SiftDown(A,i):
    while true:
        best = i
        for j = 0,...,d-1:
            c = Child(i,j)
            if c >= A.heap_size:
                break
            if A[c] < A[best]:
                best = c
        if best == i:
            return
        swap A[i], A[best]
        i = best
```
Only edges descending from the moved entry can violate [heap order](../../../../../heap-order.md). If the entry is no larger than every child, the entire heap is valid. Otherwise swapping with a minimum child restores the order at the old position: that child is no larger than the old entry or any sibling. Its original subtree was already ordered, so only the moved entry's new outgoing edges can remain invalid. This is the [loop invariant](../../../../../loop-invariant.md) of `SiftDown`. Each swap moves it down one level, proving termination and correctness.

For $2\leq d\leq n$, the height is $O(\log_d n)$, and selecting a minimum child costs at most $d$ comparisons per level. Thus **`ExtractMin` takes $O(d\log_d n)$ time**, with $O(1)$ auxiliary storage. Empty and singleton heaps take constant time. For $d>n$, there is at most one nonroot level and the loop examines at most $n-1$ actual children, taking $O(n)$; this also lies within $O(d\log_d n)$ for $n\geq2$. The coarser uniform expression $O(1+d(1+\log_d n))$ safely includes all small sizes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

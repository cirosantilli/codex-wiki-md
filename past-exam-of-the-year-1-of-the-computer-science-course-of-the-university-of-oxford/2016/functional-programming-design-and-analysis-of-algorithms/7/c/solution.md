<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A decreased key can violate [heap order](../../../../../heap-order.md) only against its parent. An inserted entry begins at the next free position and uses the same repair:
```
DecreaseKey(A,i,key):
    if i < 0 or i >= A.heap_size:
        error "invalid index"
    if key > A[i]:
        error "key increased"
    A[i] = key
    while i > 0:
        p = Parent(i)
        if A[p] <= A[i]:
            return
        swap A[p], A[i]
        i = p

Insert(A,key):
    ensure capacity for A.heap_size+1 entries
    i = A.heap_size
    A.heap_size = A.heap_size+1
    A[i] = +infinity
    DecreaseKey(A,i,key)
```
Here $+\infty$ is a sentinel at least as large as every permitted key. One can equivalently write `key` directly into the new entry and run the upward loop, avoiding any sentinel representation.

At every upward swap, the smaller key moves above its larger parent; the displaced parent remains no larger than the entries below it, as follows from the old [heap order](../../../../../heap-order.md). Thus only the new parent edge can be invalid. At most one parent comparison is needed per level, with no scan of siblings. Both operations take **$O(\log_d n)$ time in the usual $2\leq d\leq n$ range**, or $O(1+\log_d(n+1))$ uniformly including tiny heaps and large $d$.

The heap-operation bound assumes space for the inserted entry. A capacity expansion in a [dynamic array](../../../../../dynamic-array.md) can cost $O(n)$ for that individual insertion; sufficient preallocation avoids it, while geometric capacity growth adds only constant amortized allocation cost per insertion.

## ↑ Ancestors (12)

1. [C](../c.md)
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

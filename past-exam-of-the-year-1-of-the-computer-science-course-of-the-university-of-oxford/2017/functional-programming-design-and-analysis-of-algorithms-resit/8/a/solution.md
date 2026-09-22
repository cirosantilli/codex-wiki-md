<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Build a [max-heap](../../../../../max-heap.md), then repeatedly swap its root with the last element of the active prefix, shrink that prefix and restore [heap order](../../../../../heap-order.md) by [heapify down](../../../../../sift-down.md). A zero-based implementation is

```
for i = floor(n/2)-1,...,0:
    siftDown(A,i,n)
for end = n-1,...,1:
    swap A[0],A[end]
    siftDown(A,0,end)
```

`siftDown(A,i,end)` repeatedly exchanges entry `i` with its larger child while the child lies below `end` and has a larger key. The suffix beyond `end` is already sorted and never touched again. For the specified input, key stages of [heapsort](../../../../../heapsort.md) are

| Stage | Active max heap | Sorted suffix |
| --- | --- | --- |
| Bottom-up heap construction | $[5,4,3,1,2]$ | $[]$ |
| Extract 5, repair | $[4,2,3,1]$ | $[5]$ |
| Extract 4, repair | $[3,2,1]$ | $[4,5]$ |
| Extract 3, repair | $[2,1]$ | $[3,4,5]$ |
| Extract 2 | $[1]$ | $[2,3,4,5]$ |

The final array is **$[1,2,3,4,5]$**. Bottom-up construction takes $O(n)$ time because there are progressively fewer nodes at each greater subtree height; the extractions give worst-case $O(n\log n)$ time and constant auxiliary storage for iterative sifting.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
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

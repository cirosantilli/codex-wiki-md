<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [maximum priority queue](../../../../../maximum-priority-queue.md) stores keyed entries and supports insertion, inspection and removal of an entry with greatest key, and key increases. A [max-heap](../../../../../max-heap.md) gives the following [running times](../../../../../running-time.md), with the size/capacity cost of the backing [array](../../../../../array-data-structure.md) accounted for separately:

- `maximum`: return the root key in **$O(1)$** time.
- `insert`: append at the next available leaf, then use [sift up](../../../../../sift-up.md) until the [heap order](../../../../../heap-order.md) holds, in **$O(\log n)$** time.
- `extractMaximum`: save the root, replace it by the last entry, reduce the size, and use [sift down](../../../../../sift-down.md), in **$O(\log n)$** time.
- `increaseKey(i,k)`: reject $k<A[i]$; otherwise set the new key and use [sift up](../../../../../sift-up.md), in **$O(\log n)$** time.
- `isEmpty` and `size`: inspect the stored size in **$O(1)$** time; construct a queue from $n$ keys by [bottom-up heap construction](../../../../../bottom-up-heap-construction.md) in **$\Theta(n)$** time.

Empty-queue inspections and removals need an explicit failure result. The index argument to `increaseKey` must identify the entry's _current_ location: if callers use item handles, update their location records during swaps.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

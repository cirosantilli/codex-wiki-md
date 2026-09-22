<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A minimum-oriented [binary heap](../../../../../../binary-heap.md) is an appropriate alternative. Store a complete [binary tree](../../../../../../binary-tree.md) in an [array](../../../../../../array-data-structure.md) and maintain [heap order](../../../../../../heap-order.md). Insertion appends a value and moves it upward; removing the root replaces it by the last value and moves that value downward. Each path has $O(\log(n+1))$ levels, and equal values can be stored in separate slots. Both operations therefore take **$O(\log(n+1))$ time when capacity is available**.

Unlike a [binary search tree](../../../../../../binary-search-tree.md), the heap does not maintain a complete search order, so finding an arbitrary specified value can require $O(n)$ inspections. A simple [array](../../../../../../array-data-structure.md) implementation also has a capacity issue: a fixed [array](../../../../../../array-data-structure.md) can fill, and resizing a growable [array](../../../../../../array-data-structure.md) occasionally costs $O(n)$, giving an amortized insertion guarantee unless allocation is otherwise managed. This capacity cost is an implementation tradeoff, not an inherent inability of heaps to represent the [priority queue](../../../../../../priority-queue.md) abstraction.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

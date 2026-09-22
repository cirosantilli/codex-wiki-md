# Best-case maximum deletion in a binary heap

↑ **Parent:** [Binary heap](binary-heap.md)

In the implementation that exchanges the root with the final leaf and then applies [heapify down](sift-down.md), a [max-heap](max-heap.md) of size at least four with distinct keys requires at least one downward exchange: the old final leaf's parent remains and has a larger key. One downward exchange can suffice, even for large heaps, by promoting the opposite root child and letting the moved key dominate that child's descendants. Thus the best case is two pairwise exchanges when the initial root/final-leaf exchange is counted. This is a convention about that implementation: a hole-moving implementation uses assignments rather than pairwise exchanges, and the worst case still has logarithmic [time complexity](time-complexity.md).

## ↑ Ancestors (5)

1. [Binary heap](binary-heap.md)
2. [Priority queue](priority-queue.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/7/c/solution.md)

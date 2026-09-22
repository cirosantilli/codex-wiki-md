# Sift down

↑ **Parent:** [Binary heap](binary-heap.md)

To repair a key in a minimum-oriented [binary heap](binary-heap.md), choose the smaller-priority present entry among its [children in a rooted tree](child-in-a-rooted-tree.md). Exchange if that entry is smaller than the moving key, and continue at the new index. Stop when there are no [children in a rooted tree](child-in-a-rooted-tree.md) or the [heap order](heap-order.md) holds. The smaller [rooted trees](rooted-tree.md) below the starting entry must already obey the [heap order](heap-order.md); choosing the larger child could leave a violation with the smaller one.

## ↑ Ancestors (5)

1. [Binary heap](binary-heap.md)
2. [Priority queue](priority-queue.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Binary heap](binary-heap.md)
- [Bottom-up heap construction](bottom-up-heap-construction.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/c/solution.md)

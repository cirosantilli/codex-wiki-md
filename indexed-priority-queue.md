# Indexed priority queue

↑ **Parent:** [Priority queue](priority-queue.md)

A [priority queue](priority-queue.md) whose entries have stable identifiers and an auxiliary map from each identifier to its current storage location. An indexed [binary heap](binary-heap.md) can therefore support membership and locating an entry in constant time, followed by a key decrease in logarithmic time. Every heap swap must update both affected map entries; otherwise later updates can modify the wrong item.

## ↑ Ancestors (4)

1. [Priority queue](priority-queue.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [D-ary min-heap](d-ary-min-heap.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/8/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/7/e/solution.md)

# d-ary min-heap

↑ **Parent:** [D-ary heap](d-ary-heap.md)

A [d-ary heap](d-ary-heap.md) in which each parent key is no greater than each child key. Transitivity makes the root a minimum. Removing the root requires choosing a smallest child at each downward step, taking $O(d\log_d n)$ time in the usual $2\leq d\leq n$ range. Decreasing a key or inserting a new leaf only compares along one chain of parents, taking $O(\log_d n)$ time in that range. These [priority queue](priority-queue.md) bounds assume constant-time key comparisons and available array capacity. An [indexed priority queue](indexed-priority-queue.md) must also update its item-to-index table after every swap.

## ↑ Ancestors (5)

1. [D-ary heap](d-ary-heap.md)
2. [Heap data structure](heap-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/7/a/solution.md)

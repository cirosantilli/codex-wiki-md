# Bottom-up heap construction

↑ **Parent:** [Binary heap](binary-heap.md)

Construct a [binary heap](binary-heap.md) from an [array](array-data-structure.md) by processing internal nodes backwards, applying [sift down](sift-down.md) at each. The [complete binary tree](complete-binary-tree.md) shape ensures that the subtrees below the current node have already been repaired. The number of nodes whose height is at least $h$ is at most $\lfloor n/2^h\rfloor$, so charging each repair by its height gives total work at most a constant multiple of $n+\sum_{h\ge1}\lfloor n/2^h\rfloor<2n$. The construction takes $\Theta(n)$ time in either heap orientation, whereas inserting entries separately has an $O(n\log n)$ worst-case bound.

## ↑ Ancestors (5)

1. [Binary heap](binary-heap.md)
2. [Priority queue](priority-queue.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/7/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/7/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/7/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/a/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)

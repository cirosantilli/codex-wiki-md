# In-place merge

↑ **Parent:** [Merge algorithm](merge-algorithm.md)

Combining adjacent [sorted runs](sorted-run.md) within their existing [array](array-data-structure.md) segment. A simple constant-auxiliary-space version moves the smaller second-run head before the first-run head by shifting the intervening block one place right. The finished prefix is always a merge of the consumed portions. This can use quadratic [running time](running-time.md); minimizing storage does not automatically preserve the linear cost of a disjoint-output merge.

## ↑ Ancestors (4)

1. [Merge algorithm](merge-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/3/f/solution.md)

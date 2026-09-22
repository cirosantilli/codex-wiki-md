# Bitonic sorting algorithm

↑ **Parent:** [Sorting algorithm](sorting-algorithm.md)

A [divide-and-conquer algorithm](divide-and-conquer-algorithm.md) that sorts two halves, reverses one result to form a [bitonic sequence](bitonic-sequence.md), then performs a bitonic merge. For the shuffle-and-adjacent-comparison merging network on $n=2^k$ entries, $k$ passes each cost $\Theta(n)$, so merging costs $\Theta(n\log n)$. The complete [recurrence relation](recurrence-relation.md) is $T(n)=2T(n/2)+\Theta(n\log n)$, giving $\Theta(n(\log n)^2)$ time. A compare-exchange operation preserves the [multiset](multiset.md) of entries while putting its two selected entries in order.

## ↑ Ancestors (4)

1. [Sorting algorithm](sorting-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/4/f/solution.md)

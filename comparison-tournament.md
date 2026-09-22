# Comparison tournament

↑ **Parent:** [Selection algorithm](selection-algorithm.md)

Pair candidates from a [totally ordered set](totally-ordered-set.md) and retain the greater one from each comparison until one winner remains. Every other candidate loses once, so $n-1$ key comparisons suffice to find the [maximum](maximum-of-a-subset-of-a-total-order.md) of $n$ distinct values. A balanced tournament on $2^m$ inputs gives the winner $m$ direct losers. Retaining each loser's own defeat record preserves information for finding later order statistics. The comparison records form a rooted tree and are distinct from a graph-theoretic [tournament](tournament-graph-theory.md), which includes a directed comparison between every pair.

**Table of contents**

- [Tournament selection of the three largest elements](tournament-selection-of-the-three-largest-elements.md)

## ↑ Ancestors (4)

1. [Selection algorithm](selection-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/5/d/solution.md)
- [Tournament selection of the three largest elements](tournament-selection-of-the-three-largest-elements.md)

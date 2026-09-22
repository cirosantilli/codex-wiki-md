# Median of medians

↑ **Parent:** [Algorithm](algorithm-split.md)

For deterministic linear-time [selection](selection-algorithm.md), group keys into fives, compute the median of each group, and recursively select the median of those medians as a pivot. Apart from bounded end effects, at least $3n/10$ keys lie on either side. Thus the selection cost satisfies $T(n)\leq T(\lceil n/5\rceil)+T(7n/10+O(1))+O(n)=O(n)$, since the fractions sum to $9/10<1$. A [strong induction](strong-induction.md) with sufficiently large linear coefficient absorbs the lower-order terms.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Lower weighted median](lower-weighted-median.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/6/c/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/5/d/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/8/c/solution.md)
- [Selection algorithm](selection-algorithm.md)

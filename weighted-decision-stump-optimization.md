# Weighted decision stump optimization

↑ **Parent:** [Decision stump](decision-stump.md)

For stumps $h(x)=\operatorname{sign}(x_i-b)$ of fixed polarity, sort observations along each coordinate and sweep the threshold across whole groups of equal values. Passing a group adds its positive-label weight and subtracts its negative-label weight from the weighted [misclassification risk](misclassification-risk.md). Include thresholds below and above all observed values. Every distinct sample prediction pattern is considered, giving exact minimization in $O(nm\log m)$ [time complexity](time-complexity.md) for $m$ observations in $\mathbb R^n$. Coordinate sort orders can be reused across [AdaBoost](adaboost.md) rounds, reducing subsequent weighted scans to $O(nm)$.

## ↑ Ancestors (8)

1. [Decision stump](decision-stump.md)
2. [Regression tree](regression-tree.md)
3. [Decision tree learning](decision-tree-learning.md)
4. [Statistical learning theory](statistical-learning-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-learning-theory/3/b/solution.md)

# Element distinctness problem

↑ **Parent:** [Computational complexity theory](computational-complexity-theory.md)

Decide whether all input elements are distinct. In the [comparison model](comparison-model.md), this needs $\Omega(n\log n)$ comparisons in the worst case. An accepting decision-tree leaf for distinct keys must force a total order: incomparable keys could otherwise be made equal consistently with its strict comparison outcomes. Thus the $n!$ possible orders require different accepting leaves, giving a decision-tree depth of at least $\log_3(n!)=\Omega(n\log n)$ even for three-way comparisons.

## ↑ Ancestors (4)

1. [Computational complexity theory](computational-complexity-theory.md)
2. [Theoretical computer science](theoretical-computer-science-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Comparison lower bound for interval disjointness](comparison-lower-bound-for-interval-disjointness.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)

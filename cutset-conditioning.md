# Cutset conditioning

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

Enumerate assignments to a [cycle cutset](cycle-cutset.md), reject internal violations, filter all crossing [binary constraints](binary-constraint.md), and solve the residual [forest](forest.md) by [tree-structured constraint satisfaction](tree-structured-constraint-satisfaction.md). A full solution restricts to one enumerated cutset assignment; the residual tree passes preserve all its values. Conversely, a consistent cutset assignment combined with supported residual solutions satisfies every constraint. These observations prove completeness and soundness.

With $n$ [variables](variable-mathematics.md), maximum [constraint domain](constraint-domain.md) size $q$ and cutset size $k$, there are at most $q^k$ assignments and $O((n-k)q^2)$ residual tree work per assignment. Internal cutset and crossing-constraint tests require additional accounting. The method is attractive when a small [cycle cutset](cycle-cutset.md) is available.[§2.4.1, Structure, cutset conditioning](cs-188-constraint-ordering-and-structure-notes.md)

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [CS 188 constraint ordering and structure notes](cs-188-constraint-ordering-and-structure-notes.md)
- [Cycle cutset](cycle-cutset.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/d/solution.md)

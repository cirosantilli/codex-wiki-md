# Full-sweep arc consistency

↑ **Parent:** [Arc consistency](arc-consistency.md)

Compute an [arc-consistency closure](arc-consistency-closure.md) by revising every directed constrained pair in complete sweeps until one sweep deletes nothing. The first sweep is unconditional. With $v$ variables, maximum [constraint domain](constraint-domain.md) size $d$, and $e$ constrained pairs, at most $vd$ deletions permit at most $vd+1$ sweeps. At $O(d^2)$ per revision plus $O(v)$ per emptiness scan, a direct [time complexity](time-complexity.md) bound is $O((vd+1)(ed^2+v))$. [AC-3](ac-3.md) uses a work list to avoid scanning unrelated arcs after each local change.

## ↑ Ancestors (8)

1. [Arc consistency](arc-consistency.md)
2. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
3. [Search problem](search-problem.md)
4. [Computational problem](computational-problem.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/b/solution.md)

# AC-3

↑ **Parent:** [Arc consistency](arc-consistency.md)

An [arc consistency](arc-consistency.md) [algorithm](algorithm-split.md) maintaining a work list of directed constrained variable pairs. Revising $i\to j$ deletes each value of $D_i$ with no compatible value in $D_j$. If $D_i$ shrinks, incoming arcs $k\to i$ are reconsidered; the just-used neighbor $j$ need not be included, since deleted values had no support in $D_j$ and hence supported no surviving value there. Initially empty [constraint domains](constraint-domain.md) are rejected before processing.

Each deletion preserves every complete solution: a solution using the removed value would supply its missing support. Therefore an empty [constraint domain](constraint-domain.md) certifies impossibility. Successful termination establishes [arc consistency](arc-consistency.md) but need not establish satisfiability. A triangle of two-valued inequality constraints supplies a counterexample: all values have pairwise support, but no assignment can satisfy all three inequalities.

For $v$ variables, $e$ constrained pairs and maximum [constraint domain](constraint-domain.md) size $d$, assume constant-time compatibility tests for combined pair relations. A revision costs $O(d^2)$, and each shrinking source [constraint domain](constraint-domain.md) can cause at most $d$ rounds of reconsideration of its incoming arcs. Thus there are $O(ed)$ revisions and [time complexity](time-complexity.md) $O(v+ed^3)$. Fixed $d$, including two-valued [constraint domains](constraint-domain.md), gives linear time in $v+e$.

## ↑ Ancestors (8)

1. [Arc consistency](arc-consistency.md)
2. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
3. [Search problem](search-problem.md)
4. [Computational problem](computational-problem.md)
5. [Computational complexity theory](computational-complexity-theory.md)
6. [Theoretical computer science](theoretical-computer-science-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Full-sweep arc consistency](full-sweep-arc-consistency.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/b/solution.md)

# Relaxation heuristic

↑ **Parent:** [Search problem](search-problem.md)

A [heuristic function](heuristic-function.md) obtained by solving an easier problem that permits every original transition and possibly additional ones, with original transitions costing no more in the easier problem. Every original solution remains available, so the easier optimum is an [admissible heuristic](admissible-heuristic.md).

If $h$ is the exact distance to the relaxed goal set, each original transition also gives $h(s)\le c(s,a,s')+h(s')$ by taking that transition and then a relaxed optimal continuation. Thus this construction gives a [consistent heuristic](consistent-heuristic.md) when original goals have relaxed distance zero. For a four-direction grid walk, deleting obstacles gives [Manhattan distance](manhattan-distance.md); deleting a pursuer's capture constraint supplies another relaxation. The resulting estimate can remain finite when the original goal is unreachable.

**Table of contents**

- [Abstraction heuristic](abstraction-heuristic.md)
  - [Pattern database](pattern-database.md)
- [Delete-relaxation heuristic](delete-relaxation-heuristic.md)

## ↑ Ancestors (6)

1. [Search problem](search-problem.md)
2. [Computational problem](computational-problem.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Admissible heuristic](admissible-heuristic.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/1/f/solution.md)

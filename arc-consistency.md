# Arc consistency

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

A directed requirement for a [binary constraint](binary-constraint.md) $R_{ij}$: every remaining $x\in D_i$ has at least one support $y\in D_j$ with $(x,y)\in R_{ij}$. Revising the arc $i\to j$ deletes unsupported values from $D_i$; it does not directly delete values from $D_j$. Full [arc consistency](arc-consistency.md) requires the condition in both directions on every [edge](edge-of-a-graph.md) of the [constraint graph](constraint-graph.md). On general [graphs](graph-split.md), it need not imply that a complete solution exists.

**Table of contents**

- [Full-sweep arc consistency](full-sweep-arc-consistency.md)
- [Arc-consistency closure](arc-consistency-closure.md)
- [AC-3](ac-3.md)

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [AC-3](ac-3.md)
- [Arc consistency](arc-consistency.md)
- [Arc-consistency closure](arc-consistency-closure.md)
- [CS 188 constraint filtering notes](cs-188-constraint-filtering-notes.md)
- [Direct SAT encoding of finite-domain constraints](direct-sat-encoding-of-finite-domain-constraints.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/2/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/3/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/3/f/solution.md)
- [Tree-structured constraint satisfaction](tree-structured-constraint-satisfaction.md)

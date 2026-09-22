# Nonattacking knights problem

↑ **Parent:** [Constraint satisfaction problem](constraint-satisfaction-problem.md)

Choose $k$ distinct squares of an $n\times n$ chessboard so that no chosen pair has absolute coordinate differences $(1,2)$ or $(2,1)$. One [constraint satisfaction problem](constraint-satisfaction-problem.md) representation has $k$ square-valued [variables](variable-mathematics.md), requiring distinctness and pairwise nonattack. Another has one [Boolean variable](boolean-variable.md) per square, a [cardinality constraint](cardinality-constraint.md) fixing their [sum](sum.md) to $k$, and one mutual-exclusion constraint for every [edge](edge-of-a-graph.md) of the [knight attack graph](knight-attack-graph.md). The first has fewer [variables](variable-mathematics.md) when $k$ is small but represents each unlabelled placement up to $k!$ times; the second uses only binary [constraint domains](constraint-domain.md) and sparse local attack restrictions.

**Table of contents**

- [Knight attack graph](knight-attack-graph.md)

## ↑ Ancestors (7)

1. [Constraint satisfaction problem](constraint-satisfaction-problem.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/2/a/solution.md)

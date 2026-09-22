# Degree branching with a one-tree bound

↑ **Parent:** [Branch and bound](branch-and-bound.md)

If a minimum [one-tree](1-tree.md) is not a tour, some vertex has degree greater than two, since there are equally many edges and vertices. Every tour must omit at least one of its incident selected edges. Partition tours by the first omitted edge in an ordered list, forcing all preceding listed edges and forbidding that edge. These disjoint children cover all tours. Recompute the constrained [one-tree](1-tree.md) [lower bound](lower-bound-in-a-partially-ordered-set.md) in each child and compare it with the [incumbent solution](incumbent-solution.md) to prune.

## ↑ Ancestors (6)

1. [Branch and bound](branch-and-bound.md)
2. [Integer programming](integer-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2010/1/c/solution.md)

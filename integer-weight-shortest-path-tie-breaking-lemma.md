# Integer-weight shortest-path tie-breaking lemma

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

In a finite graph with positive integral [edge](edge-of-a-graph.md) weights, replacing $w(e)$ by $|V|w(e)+1$ makes every transformed [shortest path](shortest-path.md) minimise original weight first and [edge](edge-of-a-graph.md) count second. Positive weights imply that an optimal route is simple, with at most $|V|-1$ [edges](edge-of-a-graph.md). Original integral path weights that differ have a gap of at least one; multiplication by $|V|$ outweighs every possible difference in simple-path [edge](edge-of-a-graph.md) counts. Among equal-weight paths, only the added [edge](edge-of-a-graph.md) count differs. Thus a single ordinary [shortest path](shortest-path.md) computation solves lexicographic weight-and-hop minimisation.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/7/c/solution.md)

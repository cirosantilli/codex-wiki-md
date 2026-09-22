# Semi-random palette refinement for triangle-free colouring

↑ **Parent:** [Graph coloring](graph-coloring.md)

Maintain lists of available colours, tentatively colour small random portions, erase conflicts and prune colours used by neighbours. In a [triangle-free graph](triangle-free-graph.md), a vertex's neighbours form an [independent set](independent-set-graph-theory.md), which enables local estimates. Track list size and average remaining neighbour congestion per colour; prune unusually congested colours before the next round. Concentration and the [Lovász local lemma](lovasz-local-lemma.md) preserve these invariants until lists have enough slack for completion. Tracking averages matters because triangle-free graphs can still contain many four-cycles and need not have uniform per-colour congestion.

## ↑ Ancestors (6)

1. [Graph coloring](graph-coloring.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/5/solution.md)

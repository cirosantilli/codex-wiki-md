# Simultaneous giant for fixed random-edge choice

↑ **Parent:** [Random graph](random-graph.md)

Offer $k$ independent uniform [edges](edge-of-a-graph.md) of the [complete graph](complete-graph.md) per row and permit any one to be selected from each row. If a chosen [graph](graph-split.md) has no [graph component](component-graph-theory.md) of order at least $2n/3$, the [balanced component cut](balanced-component-cut.md) provides an empty cut whose sides both have at least $n/3$ [vertices](vertex-graph-theory.md). Each candidate [edge](edge-of-a-graph.md) crosses that cut with [probability](probability.md) at least $4/9$, so a row can avoid crossing with [probability](probability.md) at most $1-(4/9)^k$. The [union bound](boole-s-inequality.md) over at most $2^n$ cuts gives failure probability at most $2^n[1-(4/9)^k]^{cn}$. Any fixed integer $c$ with $c[-\log(1-(4/9)^k)]>\log2$ suffices. The guarantee is simultaneous even for choices made after seeing every offered [edge](edge-of-a-graph.md).

## ↑ Ancestors (6)

1. [Random graph](random-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/2/ii/solution.md)

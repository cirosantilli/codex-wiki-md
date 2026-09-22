# Forced merging of large components

↑ **Parent:** [Achlioptas process](achlioptas-process.md)

For the two-choice [Achlioptas process](achlioptas-process.md), fix $a>0$ and $K\geq1$. Conditional on any current [graph](graph-split.md) with $N_{\geq K}\geq an$, put $W$ equal to the [vertices](vertex-graph-theory.md) in its large [graph components](component-graph-theory.md). There are at most $n/K$ such initial [graph components](component-graph-theory.md). If after $s$ more steps no [graph component](component-graph-theory.md) contains $an/3$ [vertices](vertex-graph-theory.md) of $W$, greedily assign final [graph components](component-graph-theory.md) to two groups so that each meets at least $|W|/3\geq an/3$ [vertices](vertex-graph-theory.md) of $W$. This induces a [set partition](set-partition.md) of the initial large [graph components](component-graph-theory.md), of which there are at most $2^{n/K}$ possibilities.

For any fixed such split $W=A\cup B$, a uniform candidate [edge](edge-of-a-graph.md) joins $A$ to $B$ with [probability](probability.md) at least $2a^2/9$. If both candidates do so, the selected [edge](edge-of-a-graph.md) cannot avoid the crossing. Thus the [probability](probability.md) that the split survives all $s$ steps is at most $(1-a^4/81)^s$. The deliberately weaker constant also covers distinct candidate sampling for sufficiently large $n$. In the absent-edge version, as long as the split has survived, every $A$--$B$ [edge](edge-of-a-graph.md) is absent, so conditioning on absence can only increase this crossing [probability](probability.md). A [union bound](boole-s-inequality.md) with $s=\lceil A(a)n/K\rceil$ and $A(a)=81(\log2+2)/a^4$ bounds failure by $e^{-2n/K}$. For fixed $K$, a further [union bound](boole-s-inequality.md) makes the conclusion simultaneous over all starting steps $m\leq3n$. This proof is independent of how the rule chooses between the two candidates.

## ↑ Ancestors (7)

1. [Achlioptas process](achlioptas-process.md)
2. [Random graph](random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Achlioptas process](achlioptas-process.md)
- [Continuity of fixed-choice percolation](continuity-of-fixed-choice-percolation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/5/i/solution.md)

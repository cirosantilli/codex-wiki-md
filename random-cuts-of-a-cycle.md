# Random cuts of a cycle

↑ **Parent:** [Cycle graph](cycle-graph.md)

Choose $r$ distinct [edges](edge-of-a-graph.md) uniformly from an $n$-vertex [cycle graph](cycle-graph.md), with $1\le r\le n$, and delete them. Two specified [vertices](vertex-graph-theory.md) at oriented distance $k$ remain connected exactly when one of their two complementary [edge-disjoint paths](edge-disjoint-paths.md) is uncut. All cuts must then lie in the other path, giving the displayed [probability](probability.md). The two events are disjoint because at least one [edge](edge-of-a-graph.md) is cut. Set $\binom ar=0$ when $a<r$.

Summing the connectivity [indicators](indicator-function.md) for all other [vertices](vertex-graph-theory.md) gives an expected number

$$
\frac{2\sum_{k=1}^{n-1}\binom kr}{\binom nr}
=\frac{2\binom n{r+1}}{\binom nr}
=\frac{2(n-r)}{r+1}
$$

of other [vertices](vertex-graph-theory.md) in a tagged [connected component](connected-component.md). The sum identity follows by classifying $(r+1)$-element [subsets](subset.md) according to their greatest element. For three cuts this is $(n-3)/2$ other [vertices](vertex-graph-theory.md).

## ↑ Ancestors (8)

1. [Cycle graph](cycle-graph.md)
2. [Cycle in a graph](cycle-in-a-graph.md)
3. [Path in a graph](path-in-a-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/7/c/i/solution.md)

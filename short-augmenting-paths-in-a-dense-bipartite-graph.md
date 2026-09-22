# Short augmenting paths in a dense bipartite graph

↑ **Parent:** [Augmenting path in a matching](augmenting-path-in-a-matching.md)

The two sides have $n$ [vertices](vertex-graph-theory.md) each. Given a nonperfect [matching in a graph](matching-graph-theory.md), choose unmatched [vertices](vertex-graph-theory.md) $u,v$ on opposite sides. An unmatched [neighbour](neighbour-of-a-vertex.md) of either supplies a one-edge [augmenting path in a matching](augmenting-path-in-a-matching.md). Otherwise their [neighbours](neighbour-of-a-vertex.md) are matched; the matched left [vertices](vertex-graph-theory.md) corresponding to $N(u)$ and the set $N(v)$ have total size greater than $n$, so they intersect. This supplies the alternating [path in a graph](path-in-a-graph.md) $u,b,a,v$ with $ab$ in the [matching in a graph](matching-graph-theory.md). Repeated augmentation produces a [perfect matching](perfect-matching.md).

Choose such an augmentation deterministically. Its reverse is specified by at most four [vertices](vertex-graph-theory.md), giving at most $2n^4$ preimages for a [matching in a graph](matching-graph-theory.md) of the next size. Thus the [matching generating function](matching-generating-function.md) coefficients satisfy $m_k\leq2n^4m_{k+1}$.

## ↑ Ancestors (7)

1. [Augmenting path in a matching](augmenting-path-in-a-matching.md)
2. [Matching (graph theory)](matching-graph-theory.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Dense permanent approximation](dense-permanent-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)

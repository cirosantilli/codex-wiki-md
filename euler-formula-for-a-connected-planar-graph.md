# Euler formula for a connected planar graph

↑ **Parent:** [Planar graph](planar-graph.md)

For a finite [connected graph](connected-graph.md) with at least one [vertex](vertex-graph-theory.md), embedded as a [plane graph](plane-graph.md), let $n$ count [vertices](vertex-graph-theory.md), $m$ count [edges](edge-of-a-graph.md), and $f$ count [faces of a plane graph](face-of-a-plane-graph.md), including the [outer face](outer-face.md). Then

$$
n-m+f=2.
$$

The hypotheses refer to an actual embedding; regions in a crossing-filled [graph drawing](graph-drawing.md) do not supply its $f$.[Planar Graphs; Bipartite Matching, slides lec 5f.14–5f.15](planar-graphs-bipartite-matching-by-albert-r-meyer-6-042j-lecture-5f.md)

In the [plane graph](plane-graph.md) $K_4$ pictured above, three bounded [faces of a plane graph](face-of-a-plane-graph.md) and the [outer face](outer-face.md) give $4-6+4=2$. A square [cycle graph](cycle-graph.md) gives $4-4+2=2$, while the [graph path](path-in-a-graph.md) $A-B-C$ gives $3-2+1=2$. Changing a crossing into a new [vertex](vertex-graph-theory.md) changes the [graph](graph-split.md): the square-and-diagonals drawing then has five [vertices](vertex-graph-theory.md), eight [edges](edge-of-a-graph.md), and five [faces of a plane graph](face-of-a-plane-graph.md), giving $5-8+5=2$.

A proof outline deletes [edges](edge-of-a-graph.md) on [graph cycles](cycle-in-a-graph.md). Each deletion preserves the [connected graph](connected-graph.md) and merges two [faces of a plane graph](face-of-a-plane-graph.md), leaving $n-m+f$ unchanged. Eventually a [tree](tree-graph-theory.md) remains, with $m=n-1$ and $f=1$. Adding the point at infinity identifies the plane picture with a [sphere](sphere.md); the value two agrees with its [Euler characteristic](euler-characteristic.md) and the [cell-count formula for Euler characteristic](cell-count-formula-for-euler-characteristic.md).

**Table of contents**

- [Small faces of a spherical polyhedral graph](small-faces-of-a-spherical-polyhedral-graph.md)
- [Planar graph edge bound](planar-graph-edge-bound.md)
  - [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
  - [Nonplanarity by edge counts](nonplanarity-by-edge-counts.md)
- [Planar girth edge bound](planar-girth-edge-bound.md)
- [Triangle-pentagon planar edge bound](triangle-pentagon-planar-edge-bound.md)
  - [Icosidodecahedral graph](icosidodecahedral-graph.md)

## ↑ Ancestors (6)

1. [Planar graph](planar-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
- [Euler formula for a sphere](euler-formula-for-a-sphere.md)
- [Five color theorem](five-color-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-3/4e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/17g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/17f/b/solution.md)
- [Planar cluster-count identity](planar-cluster-count-identity.md)
- [Planar graph edge bound](planar-graph-edge-bound.md)
- [Small faces of a spherical polyhedral graph](small-faces-of-a-spherical-polyhedral-graph.md)
- [Triangle-pentagon planar edge bound](triangle-pentagon-planar-edge-bound.md)

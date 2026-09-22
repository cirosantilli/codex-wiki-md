# Planar graph

↑ **Parent:** [Graph theory](graph-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Planar_graph)

A [planar graph](planar-graph.md) admits at least one [graph drawing](graph-drawing.md) in which [edges](edge-of-a-graph.md) meet only at common endpoints. This is a property of the abstract [graph](graph-split.md), not a requirement on every [graph drawing](graph-drawing.md). A [plane graph](plane-graph.md) specifies one such drawing.[Planar Graphs; Bipartite Matching, slides lec 5f.3 and 5f.12](planar-graphs-bipartite-matching-by-albert-r-meyer-6-042j-lecture-5f.md)

For example, the [complete graph](complete-graph.md) $K_4$ joins every pair of four [vertices](vertex-graph-theory.md), giving six [edges](edge-of-a-graph.md). Put its [vertices](vertex-graph-theory.md) at the corners of a square and its diagonals cross. Instead put $A,B,C$ at the corners of a [triangle](triangle.md) and $D$ inside it: the same six [edges](edge-of-a-graph.md) $AB,AC,BC,AD,BD,CD$ now meet only at their endpoints. The first [graph drawing](graph-drawing.md) obscures planarity; the second proves it. In particular, its [crossing number](crossing-number.md) is zero.

<a id="complete-four-vertex-graph-crossing-and-plane-drawings"></a>
![](complete-four-vertex-graph-crossing-and-plane-drawings.png)

**[Figure 30](#complete-four-vertex-graph-crossing-and-plane-drawings). The same complete graph on four vertices drawn with a crossing and with four faces**.

The distinction matters whenever connections must fit on one surface without intersecting. A failed [graph drawing](graph-drawing.md) may only need rearrangement, whereas [nonplanarity by edge counts](nonplanarity-by-edge-counts.md) proves that every rearrangement fails.

**Table of contents**

- [Kuratowski's theorem](kuratowski-s-theorem.md)
- [Plane graph](plane-graph.md)
  - [Face of a plane graph](face-of-a-plane-graph.md)
    - [Outer face](outer-face.md)
    - [Facial boundary walk](facial-boundary-walk.md)
- [Honeycomb lattice](honeycomb-lattice.md)
  - [Martini lattice](martini-lattice.md)
- [Four color theorem](four-color-theorem.md)
- [Five color theorem](five-color-theorem.md)
- [Planar map](planar-map.md)
  - [Face of a planar map](face-of-a-planar-map.md)
  - [Rooted planar map](rooted-planar-map.md)
  - [Planar quadrangulation](planar-quadrangulation.md)
    - [Trivial bijection between planar maps and quadrangulations](trivial-bijection-between-planar-maps-and-quadrangulations.md)
- [Planar dual graph](planar-dual-graph.md)
  - [Planar cluster-count identity](planar-cluster-count-identity.md)
  - [Dual bond percolation](dual-bond-percolation.md)
    - [Three-terminal cell partition duality](three-terminal-cell-partition-duality.md)
    - [Dual contour bound for a finite planar cluster](dual-contour-bound-for-a-finite-planar-cluster.md)
  - [Planar duality for rectangle crossings](planar-duality-for-rectangle-crossings.md)
    - [Exact self-dual rectangle crossing probability](exact-self-dual-rectangle-crossing-probability.md)
- [Euler formula for a connected planar graph](euler-formula-for-a-connected-planar-graph.md)
  - [Small faces of a spherical polyhedral graph](small-faces-of-a-spherical-polyhedral-graph.md)
  - [Planar graph edge bound](planar-graph-edge-bound.md)
    - [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
    - [Nonplanarity by edge counts](nonplanarity-by-edge-counts.md)
  - [Planar girth edge bound](planar-girth-edge-bound.md)
  - [Triangle-pentagon planar edge bound](triangle-pentagon-planar-edge-bound.md)
    - [Icosidodecahedral graph](icosidodecahedral-graph.md)

## ↑ Ancestors (5)

1. [Graph theory](graph-theory-split.md)
2. [Foundations of mathematics](foundations-of-mathematics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Bipartite planar graph edge bound](bipartite-planar-graph-edge-bound.md)
- [Chordal graph](chordal-graph.md)
- [Five color theorem](five-color-theorem.md)
- [Four color theorem](four-color-theorem.md)
- [Four-connected planar obstruction to two-linkage](four-connected-planar-obstruction-to-two-linkage.md)
- [Graph minor](graph-minor.md)
- [Graph subdivision](graph-subdivision.md)
- [Honeycomb lattice](honeycomb-lattice.md)
- [Kuratowski's theorem](kuratowski-s-theorem.md)
- [Martini lattice](martini-lattice.md)
- [Nonplanarity by edge counts](nonplanarity-by-edge-counts.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/17g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/17g/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-161/1/i/solution.md)
- [Planar graph](planar-graph.md)
- [Planar graph edge bound](planar-graph-edge-bound.md)
- [Planar map](planar-map.md)
- [Plane graph](plane-graph.md)
- [Self-dual parameter of the random-cluster model](self-dual-parameter-of-the-random-cluster-model.md)
- [Small faces of a spherical polyhedral graph](small-faces-of-a-spherical-polyhedral-graph.md)
- [Topological minor](topological-minor.md)

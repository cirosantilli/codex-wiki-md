# Euler circuit

↑ **Parent:** [Eulerian graph](eulerian-graph.md)

An [Euler circuit](euler-circuit.md), also called an [Euler tour](euler-circuit.md), is an [Eulerian trail](eulerian-trail.md) whose final [vertex](vertex-graph-theory.md) equals its initial [vertex](vertex-graph-theory.md). Its length is $|E|$. It can revisit other [vertices](vertex-graph-theory.md), unlike a [Hamiltonian cycle](hamilton-cycle.md), which visits each [vertex](vertex-graph-theory.md) once before returning to the start. For a finite undirected [multigraph](multigraph.md) with at least one [edge](edge-of-a-graph.md), an [Euler circuit](euler-circuit.md) exists exactly when the [edge support of a graph](edge-support-of-a-graph.md) is a [connected graph](connected-graph.md) and every [vertex degree](degree-graph-theory.md) is even.

For example, let $p,q$ be distinct parallel [edges](edge-of-a-graph.md) joining $A,B$, let $\ell$ be a [self-loop](loop-graph-theory.md) at $A$, and add an [isolated vertex](isolated-vertex.md) $Z$. Then $(\deg(A),\deg(B),\deg(Z))=(4,2,0)$, and $A,\ell,A,p,B,q,A$ is an [Euler tour](euler-circuit.md). The [self-loop](loop-graph-theory.md) supplies one traversal and two incidences; $Z$ need not be visited. Replacing $p,q$ by a single [edge](edge-of-a-graph.md) changes both [vertex degrees](degree-graph-theory.md) to odd numbers and removes the possibility of an [Euler circuit](euler-circuit.md). Thus collapsing parallel [edges](edge-of-a-graph.md) can change the answer.

Two [triangles in a graph](triangle-in-a-graph.md) sharing one [vertex](vertex-graph-theory.md) $A$ give another instructive [Euler circuit](euler-circuit.md): $A,B,C,A,D,E,A$. The shared [vertex](vertex-graph-theory.md) has [vertex degree](degree-graph-theory.md) four, the others have [vertex degree](degree-graph-theory.md) two, and $A$ is revisited between the two closed [trails](trail-in-a-graph.md). This is precisely the splice used by [Hierholzer's algorithm](hierholzer-s-algorithm.md).

## ↑ Ancestors (6)

1. [Eulerian graph](eulerian-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Christofides algorithm](christofides-algorithm.md)
- [Closed walk](closed-walk.md)
- [Double-tree approximation for metric TSP](double-tree-approximation-for-metric-tsp.md)
- [Edge support of a graph](edge-support-of-a-graph.md)
- [Euler circuit](euler-circuit.md)
- [Euler circuit criterion](euler-circuit-criterion.md)
- [Eulerian graph](eulerian-graph.md)
- [Eulerian trail](eulerian-trail.md)
- [Hamilton cycle](hamilton-cycle.md)
- [Hierholzer's algorithm](hierholzer-s-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-42/3/c/solution.md)
- [Weighted Hamilton cycle](weighted-hamilton-cycle.md)

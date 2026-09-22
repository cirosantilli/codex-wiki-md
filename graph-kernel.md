# Graph kernel

↑ **Parent:** [2-core of a graph](2-core-of-a-graph.md)

For a [connected graph](connected-graph.md) whose [2-core](2-core-of-a-graph.md) contains a [vertex](vertex-graph-theory.md) of [degree of a vertex](degree-graph-theory.md) at least three, suppress each maximal [graph path](path-in-a-graph.md) with degree-two internal [vertices](vertex-graph-theory.md) to a single [edge](edge-of-a-graph.md), allowing its two endpoints to coincide. Here suppression is the reverse of [graph subdivision](graph-subdivision.md). The resulting [multigraph](multigraph.md), retaining [self-loops](loop-graph-theory.md) and parallel [edges](edge-of-a-graph.md), is its [graph kernel](graph-kernel.md). Each suppressed internal [vertex](vertex-graph-theory.md) removes one [vertex](vertex-graph-theory.md) and one [edge](edge-of-a-graph.md), preserving [graph excess](graph-excess.md); counting a [self-loop](loop-graph-theory.md) twice toward [degree of a vertex](degree-graph-theory.md), every remaining [vertex](vertex-graph-theory.md) has [degree of a vertex](degree-graph-theory.md) at least three. A purely cyclic [2-core](2-core-of-a-graph.md) is a separate unicyclic case: it has no branching [vertex](vertex-graph-theory.md) to anchor this construction.

For the barbell in [bridges and connectivity in the 2-core](bridges-and-connectivity-in-the-2-core.md), the [graph kernel](graph-kernel.md) has two [vertices](vertex-graph-theory.md) $c,d$, one [self-loop](loop-graph-theory.md) at each, and a single joining [edge](edge-of-a-graph.md) $cd$. Suppressing $x,y$ contracts the joining [graph path](path-in-a-graph.md) to that [bridge in a graph](bridge-graph-theory.md); suppressing the two other [vertices](vertex-graph-theory.md) on each triangle turns the triangle into a [self-loop](loop-graph-theory.md). The [graph excess](graph-excess.md) stays $9-8=3-2=1$. Thus forming a [graph kernel](graph-kernel.md) compresses degree-two chains rather than deleting everything outside [graph cycles](cycle-in-a-graph.md).

## ↑ Ancestors (6)

1. [2-core of a graph](2-core-of-a-graph.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Bicyclic graph](bicyclic-graph.md)
- [Bicyclic kernel classification](bicyclic-kernel-classification.md)
- [Bridges and connectivity in the 2-core](bridges-and-connectivity-in-the-2-core.md)
- [Graph kernel](graph-kernel.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/ii/solution.md)

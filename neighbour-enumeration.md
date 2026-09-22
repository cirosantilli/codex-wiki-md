# Neighbour enumeration

↑ **Parent:** [Adjacency list](adjacency-list.md)

[Neighbour enumeration](neighbour-enumeration.md) reports the [neighbours](neighbour-of-a-vertex.md) of a specified [vertex](vertex-graph-theory.md). For a [simple graph](simple-graph.md), scan its [adjacency list](adjacency-list.md) and report each entry. With constant-time list access and work per entry, a list of length $d$ needs $O(1+d)$ time in [Big O notation](big-o-notation.md), conventionally written $O(d)$ for nonempty lists. Use [vertex degree](degree-graph-theory.md) for an [undirected graph](undirected-graph.md) and [outdegree](outdegree.md) for a [directed graph](directed-graph.md). Obtaining the list reference can take constant time; consuming it requires visiting every entry.[Digraph.java, class documentation and adj: obtaining the collection versus iterating in time proportional to outdegree](algorithms-4th-edition-by-robert-sedgewick-and-others/digraph-java.md)

In our undirected example, enumerating $C$'s [neighbours](neighbour-of-a-vertex.md) reads $A,B,D$: three entries. Scanning row $C$ of the full [adjacency matrix](adjacency-matrix.md) reads six entries, $(1,1,0,1,0,0)$, to produce the same answer. In the directed variant, enumerating $F$'s outgoing [neighbours](neighbour-of-a-vertex.md) reads no neighbour entries, but still needs constant work to locate and recognize its empty list. For a [multigraph](multigraph.md), scanning lists enumerates incident [edges](edge-of-a-graph.md) with multiplicity; reporting only distinct [neighbours](neighbour-of-a-vertex.md) additionally requires removing repetitions.

For a short [time complexity](time-complexity.md) argument, each reported entry requires at least one output operation, and one scan suffices. Across all [vertices](vertex-graph-theory.md), the undirected entry count is $\sum_{v\in V}\deg(v)=2|E|$ by the [handshaking lemma](degree-sum-formula.md); the directed count is $\sum_{v\in V}d^+(v)=|E|$. A [graph search](graph-search.md) that processes each [vertex](vertex-graph-theory.md) once and scans each of its entries once therefore does $O(|V|+|E|)$ structural work, provided its visited-state access and [FIFO queue](fifo-queue.md) or [stack](stack-data-structure.md) operations also have the required constant-time costs. With a full [adjacency matrix](adjacency-matrix.md), scanning every row instead inspects $|V|^2$ entries. This is how the representation enters the analysis of [breadth-first search](breadth-first-search.md) and [depth-first search](depth-first-search.md).

## ↑ Ancestors (4)

1. [Adjacency list](adjacency-list.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Adjacency list](adjacency-list.md)
- [Adjacency list storage and query costs](adjacency-list-storage-and-query-costs.md)
- [Neighbour enumeration](neighbour-enumeration.md)

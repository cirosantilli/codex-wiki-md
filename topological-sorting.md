# Topological sorting

↑ **Parent:** [Directed acyclic graph](directed-acyclic-graph.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Topological_sorting)

A [topological sorting](topological-sorting.md) is the task of constructing a [topological order](topological-order.md) of a finite [directed graph](directed-graph.md), or reporting that a [directed cycle](directed-cycle.md) makes one impossible. [Kahn's algorithm](kahn-s-algorithm.md) repeatedly takes a [vertex](vertex-graph-theory.md) with no unfinished prerequisites. This is useful whenever an operation consumes results produced by earlier operations: once a [vertex](vertex-graph-theory.md) is reached in a [topological order](topological-order.md), every prerequisite along a [directed path](directed-path.md) has already been processed. [MIT, Lecture 14: job scheduling and topological sorting](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2008/resources/lec14/)

The reason a choice is always available in a nonempty finite [Directed acyclic graph](directed-acyclic-graph.md) is simple. If every [vertex](vertex-graph-theory.md) had an incoming [directed edge](directed-edge.md), repeatedly following predecessors would eventually revisit a [vertex](vertex-graph-theory.md), giving a [directed cycle](directed-cycle.md). Removing a [vertex](vertex-graph-theory.md) and its incident [directed edges](directed-edge.md) cannot create a [directed cycle](directed-cycle.md), so the argument repeats until every [vertex](vertex-graph-theory.md) is listed. This proves existence of a [topological order](topological-order.md) and explains why finiteness matters to this procedure.

// Target: combinatorics.bigb

**Table of contents**

- [Topological order](topological-order.md)
- [Kahn's algorithm](kahn-s-algorithm.md)

## ↑ Ancestors (5)

1. [Directed acyclic graph](directed-acyclic-graph.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Critical path method](critical-path-method.md)
- [Directed acyclic graph](directed-acyclic-graph.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Topological order](topological-order.md)
- [Topological ordering](topological-ordering.md)
- [Topological sorting](topological-sorting.md)

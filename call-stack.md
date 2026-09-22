# Call stack

↑ **Parent:** [Stack (data structure)](stack-data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Call_stack)

A [call stack](call-stack.md) stores active procedure calls and the information needed to resume each caller, such as its return location and local variables. A call adds a frame; returning removes that frame and resumes the previous call. When [depth-first search](depth-first-search.md) uses [recursion](recursion-computer-science.md), a frame also records where its [adjacency list](adjacency-list.md) scan paused. The active frames describe a [graph path](path-in-a-graph.md) from the starting [vertex](vertex-graph-theory.md) to the current [vertex](vertex-graph-theory.md); finished calls have left the [call stack](call-stack.md), although their [vertices](vertex-graph-theory.md) remain marked as discovered.

## ↑ Ancestors (4)

1. [Stack (data structure)](stack-data-structure.md)
2. [Data structure](data-structure.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Breadth-first search](breadth-first-search.md)
- [Cached cell value](cached-cell-value.md)
- [Call stack](call-stack.md)
- [Depth-first search](depth-first-search.md)
- [Execution context](execution-context.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Stack pointer](stack-pointer.md)
- [Thread (computing)](thread-computing.md)

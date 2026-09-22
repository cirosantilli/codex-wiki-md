# Stack (data structure)

↑ **Parent:** [Data structure](data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stack_(abstract_data_type))

A [stack](stack-data-structure.md) is a [data structure](data-structure.md) with last-in, first-out behavior: `push` adds an item at the top, `pop` removes and returns the top item, and `peek` inspects it without removal. Push $A,B,C$: successive removals return $C,B,A$. Inspection and removal require a nonempty [stack](stack-data-structure.md), or a specified empty-case result. A [linked list](linked-list.md) whose head is the top supports all three operations in $O(1)$ worst-case time under constant-cost pointer operations and allocation. The [stack](stack-data-structure.md) interface itself does not fix these costs. [Sedgewick and Wayne, Algorithms: Stack interface and implementation](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/Stack.java)

A [stack](stack-data-structure.md) records work that must be resumed in reverse order: the most recent unfinished task is handled first. [Depth-first search](depth-first-search.md) uses this discipline to finish a newly entered branch before resuming the older branch that led to it. [Breadth-first search](breadth-first-search.md) uses a [FIFO queue](fifo-queue.md) to resume the oldest pending [vertex](vertex-graph-theory.md) instead. Both are small interfaces whose removal rule changes the shape of a [graph search](graph-search.md).

**Table of contents**

- [Call stack](call-stack.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

# Deque endpoint invariant

↑ **Parent:** [Double-ended queue](double-ended-queue.md)

In an endpoint-based doubly linked deque, the two endpoint references are simultaneously null exactly in the empty state. Otherwise the first predecessor and last successor are null, the finite chain is acyclic, and neighbouring links are [reciprocal](multiplicative-inverse.md). Following successors and predecessors gives the same nodes in reverse order. Removing the sole node must therefore clear both endpoints; merely clearing the one used by the operation is insufficient.

## ↑ Ancestors (4)

1. [Double-ended queue](double-ended-queue.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

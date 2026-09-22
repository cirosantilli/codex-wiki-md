# Circular buffer operation costs

↑ **Parent:** [Circular buffer](circular-buffer.md)

With storage allocated in advance, each successful insertion, removal, `peek`, `size`, and full/empty check uses $O(1)$ worst-case [time complexity](time-complexity.md) in [Big O notation](big-o-notation.md). This assumes constant-cost indexed [array](array-data-structure.md) access, bounded [machine word](machine-word.md) index arithmetic and fixed-cost scalar item reads and writes. Each operation touches a bounded number of slots and fields regardless of $n$ and $C$; no shifting, scanning or resizing occurs. Rejected operations also take constant work. Producing a copy of all $n$ live items takes $O(n)$ work under the same scalar-cost assumptions.

The preallocated [array](array-data-structure.md) occupies $O(C)$ scalar slots plus constant bookkeeping. Allocation and any initial slot construction are separate setup costs. Copying a large item, running an expensive destructor or callback, allocating an item, or growing a [dynamic array](dynamic-array.md) changes the operation cost and must be charged separately. The bound is worst-case structural work, with no need for [amortized analysis](amortized-analysis.md), and says nothing about a measured wall-clock deadline.

These formulas describe sequential calls. Wrapping [array indices](array-index.md) implies neither [atomic operations](atomic-operation.md) nor safe access from multiple [software threads](thread-computing.md). Publication of an item's contents and reuse of its slot require a protocol justified under the relevant [memory model](memory-model.md), including any necessary [acquire-release synchronization](acquire-release-synchronization.md). The kernel documentation discusses barriers under explicit producer/consumer restrictions; Boost's documentation separately requires [mutual exclusion](mutual-exclusion.md) for shared access involving writes. Neither property follows merely from choosing a [circular buffer](circular-buffer.md).[David Howells and Paul E. McKenney, Circular Buffers, Using memory barriers with circular buffers; The producer; The Consumer: explicit synchronization and ordering requirements](circular-buffers-by-david-howells-and-paul-e-mckenney.md)[Jan Gaspar, Boost.Circular Buffer, Implementation, Thread-Safety: shared access involving a writer requires mutual exclusion](boost-circular-buffer-by-jan-gaspar/implementation.md)

## ↑ Ancestors (4)

1. [Circular buffer](circular-buffer.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

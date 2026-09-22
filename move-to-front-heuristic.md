# Move-to-front heuristic

↑ **Parent:** [Linked list](linked-list.md)

After a successful search in a [linked list](linked-list.md), detach the found [linked list node](linked-list-node.md) and insert that same [linked list node](linked-list-node.md) at the front. An immediate repetition of that search then succeeds after one key comparison. This helps workloads with temporal locality, though it need not reduce the cost of the search that triggers the move.

A [dummy header node](sentinel-node.md) lets a search return the found node's predecessor. If that predecessor is already the header, do nothing; otherwise bypass the found node, point it at the old first real node, and point the header at it. This preserves each key/value binding and avoids allocation. It preserves a [dictionary](associative-array.md) abstraction whose ordering is unobservable, but generally changes the abstraction of an ordered [list](list-abstract-data-type.md).

## ↑ Ancestors (4)

1. [Linked list](linked-list.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/3/g/solution.md)

# In-place linked-list reversal

↑ **Parent:** [Linked list](linked-list.md)

Reverse a finite acyclic [linked list](linked-list.md) using a reversed-prefix head and an untouched-suffix head. Save the suffix head's old successor, redirect its successor to the prefix, then advance both heads. If $P$ and $Q$ are the current sequences of node identities and $S$ the original sequence, the [loop invariant](loop-invariant.md) is $reverse(P)\mathbin{++}Q=S$, with the two reachable node sets disjoint and all payload fields unchanged. Moving $q$ from $Q=q:Q'$ to $q:P$ preserves this equation. The suffix length decreases, and at exit the prefix is exactly the reversed original list. The method takes linear [running time](running-time.md) and constant [auxiliary space](auxiliary-space.md), reusing the original nodes.

## ↑ Ancestors (4)

1. [Linked list](linked-list.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/4/c/solution.md)

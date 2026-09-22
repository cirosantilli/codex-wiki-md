# Persistent data structure

↑ **Parent:** [Data structure](data-structure-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Persistent_data_structure)

A [data structure](data-structure-split.md) whose previous versions remain usable after an update. An immutable representation can return a new root while retaining old roots. Persistence is a version-availability property; it does not require copying the whole structure, and it does not by itself guarantee a particular [time complexity](time-complexity.md) or [space complexity](space-complexity.md).

Path copying in a balanced [tree](tree-graph-theory-split.md) can preserve old versions while allocating only the updated root-to-leaf path. A [linked list](linked-list.md) can share an unchanged suffix but may copy a long prefix for a positional edit. Retained versions extend the lifetime of their reachable data, which matters when comparing snapshot history with edit-specific inverse commands.

**Table of contents**

- [Covariant persistent multiset](covariant-persistent-multiset.md)
- [Structural sharing](structural-sharing.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/c/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/imperative-programming/6/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/imperative-programming-resit/6/c/ii/solution.md)

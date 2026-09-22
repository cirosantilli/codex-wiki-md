# Memoized iterator snapshot

↑ **Parent:** [Iterator snapshot](iterator-snapshot.md)

Represent a generated [sequence](sequence.md) by shared memoized [lazy list](lazy-list.md) cells and let each iterator hold its own current cell reference. Copy that reference into a new iterator object. Advancing one cursor changes no other cursor, while every cell's future tail is generated once. Thus even a privately stateful generator can supply identical future values to independently consumed snapshots, provided its state is owned by this shared sequence and not mutated externally. Retained older cursors can keep cached prefixes alive. [Opening description and memoization example](scala-2-12-stream-api-documentation.md)

**Table of contents**

- [Memoized successor chain for stateful iterator copies](memoized-successor-chain-for-stateful-iterator-copies.md)

## ↑ Ancestors (5)

1. [Iterator snapshot](iterator-snapshot.md)
2. [Iterator](iterator.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/7/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/6/c/solution.md)

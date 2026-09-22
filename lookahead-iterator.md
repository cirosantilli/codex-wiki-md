# Lookahead iterator

↑ **Parent:** [Iterator](iterator.md)

An [iterator](iterator.md) that physically consumes and caches source elements to determine whether another logical result exists. A prepared optional result makes repeated availability queries idempotent. This is useful when a result requires a complete group of source elements and the underlying [iterator](iterator.md) exposes neither its remaining length nor a rewind operation. Source consumption is owned by the wrapper; clients must not independently advance the underlying [iterator](iterator.md).

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/7/a/solution.md)

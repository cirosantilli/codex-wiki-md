# Stateless iterator

↑ **Parent:** [Iterator](iterator.md)

An [iterator](iterator.md) whose future observable [sequence](sequence.md) can be produced without changing cursor state. An infinite constant [sequence](sequence.md) is an example: removing its first element leaves the same [sequence](sequence.md). A permanently empty [iterator](iterator.md) is another. Such cases show why an [iterator](iterator.md) interface does not logically force every implementing object to be mutable, although ordinary finite nonempty traversals need progress state somewhere.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

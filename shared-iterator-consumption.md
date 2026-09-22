# Shared iterator consumption

↑ **Parent:** [Iterator](iterator.md)

Two wrappers referring to the same destructive [iterator](iterator.md) share its remaining [sequence](sequence.md). Their local wrapper fields do not duplicate the underlying consumption state. If one wrapper drains the shared source, a later consumer sees exhaustion. Correct reasoning must therefore track aliases and the actual demand order rather than combine the outputs of imagined independent traversals.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Iterator snapshot](iterator-snapshot.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/6/a/solution.md)

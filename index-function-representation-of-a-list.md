# Index-function representation of a list

↑ **Parent:** [List (abstract data type)](list-abstract-data-type.md)

Represent a finite [list](list-abstract-data-type.md) by a [function](function-split.md) from indices to [optional values](optional-value.md). There must be a length $m$ for which exactly the indices $0\leq i<m$ are present; later indices are absent, so the representation has no holes. Prepending and removing a head shift indices, taking restricts the present domain, and dropping translates it. Functional composition can accumulate query costs, so [array](array-data-structure.md)-like constant-time access does not follow from the representation type.

## ↑ Ancestors (4)

1. [List (abstract data type)](list-abstract-data-type.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

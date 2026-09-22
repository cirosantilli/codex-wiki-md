# Covariant persistent multiset

↑ **Parent:** [Persistent data structure](persistent-data-structure.md)

An immutable [multiset](multiset.md) can expose a [covariant type parameter](covariant-type-parameter.md) because reading an element only produces that type. Addition accepts a new type parameter with a [lower type bound](lower-type-bound.md), `add[U >: T](x: U)`, and returns a new `ISet[U]`. The old `ISet[T]` retains its contents and original element guarantee. Deletion returns both the removed value and a new remaining multiset; it does not mutate the old one. Duplicate occurrences are preserved.

## ↑ Ancestors (4)

1. [Persistent data structure](persistent-data-structure.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/8/c/solution.md)

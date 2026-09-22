# Golden rule for container algorithms

↑ **Parent:** [Hypergraph container](hypergraph-container.md)

A container algorithm may use membership in the unknown independent set only through information recorded in its [container fingerprint](container-fingerprint.md). With a deterministic ordering and deterministic tests, record every positive queried vertex; queried negative vertices can be excluded. All state updates must be recoverable from the fingerprint alone, so replaying the algorithm constructs a container without knowing the independent set.

## ↑ Ancestors (8)

1. [Hypergraph container](hypergraph-container.md)
2. [Hypergraph independent set](hypergraph-independent-set.md)
3. [Hypergraph](hypergraph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Container fingerprint](container-fingerprint.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-110/4/solution.md)

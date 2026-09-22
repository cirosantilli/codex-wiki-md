# Memoized successor chain for stateful iterator copies

↑ **Parent:** [Memoized iterator snapshot](memoized-iterator-snapshot.md)

Represent each generated [sequence](sequence.md) position by an immutable head and a lazily memoized successor, and give each [iterator](iterator.md) its own pointer into the shared chain. Computing a successor invokes the privately owned generator once; lagging copies reuse that same successor. Consequently a mutable [programming closure](closure-computer-programming.md) generating [Fibonacci numbers](fibonacci-number.md) can support interleaved independent cursor positions. Sharing only the generator and a copied current value would instead consume the generator's mutable state twice. This construction can retain all cells between the fastest and slowest live cursors; it does not guarantee constant [memory usage](memory-usage.md).

## ↑ Ancestors (6)

1. [Memoized iterator snapshot](memoized-iterator-snapshot.md)
2. [Iterator snapshot](iterator-snapshot.md)
3. [Iterator](iterator.md)
4. [Data structure](data-structure-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/6/c/solution.md)

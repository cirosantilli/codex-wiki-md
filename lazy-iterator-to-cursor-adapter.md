# Lazy iterator-to-cursor adapter

↑ **Parent:** [Lazy evaluation](lazy-evaluation.md)

Represent a cursor by an underlying consuming [iterator](iterator.md) plus an optional cached head. Without a cache, its abstract sequence is the iterator's sequence; with cached $v$, it is $[v]$ concatenated with the remaining iterator sequence. `current` fetches and caches exactly one value when needed, repeated reads reuse it, and advance discards it. Availability testing need not fetch a value, and construction need not query the input. This avoids forcing a future stream element that the client may never request.

## ↑ Ancestors (5)

1. [Lazy evaluation](lazy-evaluation.md)
2. [Programming language semantics](programming-language-semantics.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/7/a/i/solution.md)

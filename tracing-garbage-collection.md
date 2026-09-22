# Tracing garbage collection

↑ **Parent:** [Garbage collection](garbage-collection.md)

A [tracing garbage collection](tracing-garbage-collection.md) implementation starts from [garbage collection roots](garbage-collection-root.md) and follows [software object](software-object.md) references. [Software objects](software-object.md) outside that reachable set can be reclaimed, including cycles that have no path from a root. A decorator or adapter holding a component reference keeps that component reachable while the wrapper remains reachable. The number of allocated [software objects](software-object.md) alone does not establish how much storage can be reclaimed.

## ↑ Ancestors (4)

1. [Garbage collection](garbage-collection.md)
2. [Computer memory](computer-memory-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/imperative-programming/8/d/i/solution.md)
- [Tracing garbage collection](tracing-garbage-collection.md)

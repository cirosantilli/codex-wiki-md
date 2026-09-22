# Partial-list interleaving obstruction

↑ **Parent:** [Partial list](partial-list.md)

No generic sequential pure [Haskell](haskell.md) operation can guarantee emission of every available input occurrence when either of two input spines may be the [bottom value](bottom-value.md). To obtain an arbitrary element, it must eventually demand one input. That input can be undefined while the other is a defined singleton, so the demand blocks the promised singleton output. Choosing the other input first reverses the counterexample. [Lazy evaluation](lazy-evaluation.md) cannot determine which computation will diverge; the positive two-stream fairness result needs [proper lazy lists](proper-lazy-list.md) or a stronger concurrent computational model.

## ↑ Ancestors (6)

1. [Partial list](partial-list.md)
2. [Lazy list](lazy-list.md)
3. [Linked list](linked-list.md)
4. [Data structure](data-structure-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/c/solution.md)

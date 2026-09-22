# Proper lazy list

↑ **Parent:** [Lazy list](lazy-list.md)

A [proper lazy list](proper-lazy-list.md) has a spine exposing either finitely many cons constructors followed by `[]`, or infinitely many cons constructors, without an undefined tail at a finite position. This is a condition on the spine: an element may itself be the [bottom value](bottom-value.md) without hiding the [list](list-abstract-data-type.md)'s constructors. A [partial list](partial-list.md) with a finite visible prefix followed by $\bot$ fails this condition. The distinction supports [productivity](stream-productivity.md) proofs that inspect constructors without evaluating the stored elements.

## ↑ Ancestors (5)

1. [Lazy list](lazy-list.md)
2. [Linked list](linked-list.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Diagonal merging of lazy lists](diagonal-merging-of-lazy-lists.md)
- [Fair enumeration](fair-enumeration.md)
- [Partial-list interleaving obstruction](partial-list-interleaving-obstruction.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/g/solution.md)
- [Proper lazy list](proper-lazy-list.md)

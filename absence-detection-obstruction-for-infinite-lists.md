# Absence-detection obstruction for infinite lists

↑ **Parent:** [Lazy list](lazy-list.md)

A generic correct scan cannot always terminate with a certificate that a value is absent from an arbitrary infinite [list](list-abstract-data-type.md). Any terminating scan observes only finitely many elements. Changing the unobserved tail to include the value preserves all its observations but invalidates the certificate. The same argument prevents certifying that no occurrence follows the last one already found. A promise such as strict ascending order can provide an independent stopping rule. This explains why mathematical occurrence sets and computed [occurrence-position representations of a sequence](occurrence-position-representation-of-a-sequence.md) need different treatment on infinite inputs.

## ↑ Ancestors (5)

1. [Lazy list](lazy-list.md)
2. [Linked list](linked-list.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Diagonal merging of lazy lists](diagonal-merging-of-lazy-lists.md)
- [Occurrence-position representation of a sequence](occurrence-position-representation-of-a-sequence.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/4/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/2/c/solution.md)

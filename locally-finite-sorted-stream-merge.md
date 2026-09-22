# Locally finite sorted-stream merge

↑ **Parent:** [Merge algorithm](merge-algorithm.md)

Compare the heads of two increasing [lazy lists](lazy-list.md), emit the smaller and advance its input, or emit one copy and advance both when the heads are equal. This preserves strict order and removes duplicates. To enumerate the entire union as a [list](list-abstract-data-type.md), each requested element must have finitely many smaller elements in the union. Without this condition, an increasing sequence tending to one can permanently precede an input element equal to two. For increasing [integer](integer-split.md) streams bounded below, finiteness below each candidate guarantees that no candidate is starved.

## ↑ Ancestors (4)

1. [Merge algorithm](merge-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/2/a/solution.md)
- [Sorted multiplicative closure stream](sorted-multiplicative-closure-stream.md)

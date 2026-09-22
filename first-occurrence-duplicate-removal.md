# First-occurrence duplicate removal

↑ **Parent:** [Duplicate removal](duplicate-removal.md)

Retain the first occurrence of each distinct value in a [list](list-abstract-data-type.md). The [right fold](list-fold.md) `foldr (\x ys -> x : filter (/= x) ys) []` preserves this order under [lazy evaluation](lazy-evaluation.md). With terminating [equality tests](equality-test.md), an infinite input containing infinitely many distinct values produces every finite output prefix. If only finitely many distinct values occur, those values appear but the remaining infinite input cannot generally be certified empty: the result has an undefined tail rather than a terminating empty [list](list-abstract-data-type.md).

## ↑ Ancestors (5)

1. [Duplicate removal](duplicate-removal.md)
2. [List (abstract data type)](list-abstract-data-type.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/3/e/solution.md)

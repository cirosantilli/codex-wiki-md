# Admissible predicate on lazy lists

↑ **Parent:** [Structural induction](structural-induction.md)

A [predicate](predicate.md) on possibly partial [lists](list-abstract-data-type.md) is admissible when it holds at the limit of every increasing chain of finite approximations on which it holds. Increasing here means replacing a [bottom value](bottom-value.md) by more defined information while retaining already defined constructors and values. This closure condition permits a property established for finite approximations to pass to an infinite [list](list-abstract-data-type.md). The predicate “the list is finite” lacks this closure: every finite prefix ending in an undefined tail is finite in extent, but their limit may have infinitely many constructors.

## ↑ Ancestors (6)

1. [Structural induction](structural-induction.md)
2. [Mathematical proof](mathematical-proof.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2005/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms-resit/1/b/solution.md)
- [Structural induction on lazy lists](structural-induction-on-lazy-lists.md)

# Stable list partition

↑ **Parent:** [Functional programming](functional-programming.md)

Split a [list](list-abstract-data-type.md) into the subsequence satisfying a [predicate](predicate.md) and the subsequence failing it, preserving relative order in both. One recursive traversal computes the pair for the tail once, evaluates the head's [predicate](predicate.md) once and prepends the head to the appropriate component. A shared irrefutable pair binding preserves lazy access to either component. Fully consuming both finite outputs takes [linear time](linear-time.md) in addition to [predicate](predicate.md) evaluation costs.

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/3/f/solution.md)

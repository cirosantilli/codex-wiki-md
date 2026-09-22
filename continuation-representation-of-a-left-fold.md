# Continuation representation of a left fold

↑ **Parent:** [Left fold](left-fold.md)

A [right fold](list-fold.md) can build a [function](function-split.md) that accepts the initial accumulator later. Its empty result is `id`; its step prepends one update before the continuation supplied by the tail. The invariant `foldr c id xs a = foldl s a xs`, quantified over all `a`, follows from the two fold equations. Both applied sides give the [bottom value](bottom-value.md) on an undefined spine; finite approximation then covers infinite [lazy lists](lazy-list.md). The larger result type retains information that a direct same-result-type fold can lose.

## ↑ Ancestors (5)

1. [Left fold](left-fold.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/1/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/1/e/solution.md)

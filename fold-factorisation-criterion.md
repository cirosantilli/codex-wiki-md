# Fold factorisation criterion

↑ **Parent:** [Functional programming](functional-programming.md)

For the pure definable functions under consideration, a function on [lazy lists](lazy-list.md) is `foldr c z` when it is a [strict function](strict-function.md), maps `[]` to `z`, and satisfies `f (x:xs) = c x (f xs)` on partial as well as total inputs. Necessity follows from the fold equations. For sufficiency, [structural induction](structural-induction.md) proves equality on finite lists and finite spines ending in the [bottom value](bottom-value.md); definable continuous functions are determined on an infinite list by those finite approximations. The important information constraint is that a step receives the tail only through its folded result. Equal folded tails must yield equal extended results when the new head is the same.

## ↑ Ancestors (4)

1. [Functional programming](functional-programming.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Direct fold obstruction for dropping a prefix](direct-fold-obstruction-for-dropping-a-prefix.md)
- [List fold](list-fold.md)
- [Partial list](partial-list.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/1/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/1/f/solution.md)

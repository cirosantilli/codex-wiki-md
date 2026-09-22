# Data constructor

↑ **Parent:** [Algebraic data type](algebraic-data-type.md)

A named way to construct one alternative of an [algebraic data type](algebraic-data-type.md). In `data Tree a = One a | Two (Tree a) (Tree a)`, `One` has [type signature](type-signature.md) `a -> Tree a` and `Two` has [type signature](type-signature.md) `Tree a -> Tree a -> Tree a`. They construct values; the [type constructor](type-constructor.md) `Tree` instead constructs types from a [type argument](type-argument.md).

## ↑ Ancestors (5)

1. [Algebraic data type](algebraic-data-type.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Algebraic data type](algebraic-data-type.md)
- [Data type](data-type.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/4/a/solution.md)
- [Tree fold](tree-fold.md)
- [Type constructor](type-constructor.md)

# Haskell iterate function

↑ **Parent:** [Haskell](haskell.md)

The [higher-order function](higher-order-function.md) `iterate :: (a -> a) -> a -> [a]`, satisfying `iterate f x = x : iterate f (f x)`. Its result begins with the initial value and continues with successive applications. [Lazy evaluation](lazy-evaluation.md) permits finite prefixes of this infinite [list](list-abstract-data-type.md) to be observed whenever the necessary applications terminate.

## ↑ Ancestors (4)

1. [Haskell](haskell.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/b/solution.md)

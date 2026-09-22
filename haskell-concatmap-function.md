# Haskell concatMap function

↑ **Parent:** [Haskell](haskell.md)

The [higher-order function](higher-order-function.md) with type `(a -> [b]) -> [a] -> [b]` and value `concat (map f xs)`. It replaces each input element by a [list](list-abstract-data-type.md) and concatenates those lists in input order. A direct definition is `concatMap f = foldr (\x rest -> f x ++ rest) []`. This formulation processes an input element's produced list once; it need not repeatedly append an already accumulated output prefix.

## ↑ Ancestors (4)

1. [Haskell](haskell.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/3/d/i/solution.md)

# Map (higher-order function)

↑ **Parent:** [Higher-order function](higher-order-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Map_(higher-order_function))

Apply a [function](function-split.md) to each element of a collection while retaining its arrangement. On [lists](list-abstract-data-type.md), `map f [] = []` and `map f (x:xs) = f x : map f xs`. Its [principal type](principal-type.md) in [Haskell](haskell.md) is `(a -> b) -> [a] -> [b]`. The element types may change independently; no [equality test](equality-test.md) or ordering of elements is required.

## ↑ Ancestors (5)

1. [Higher-order function](higher-order-function.md)
2. [Functional programming](functional-programming.md)
3. [Programming language](programming-language-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

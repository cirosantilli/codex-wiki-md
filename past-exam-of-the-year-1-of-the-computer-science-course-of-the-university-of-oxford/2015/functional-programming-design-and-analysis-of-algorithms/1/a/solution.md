<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [principal types](../../../../../principal-type.md) and definitions are:
```
map :: (a -> b) -> [a] -> [b]
map _ []     = []
map f (x:xs) = f x : map f xs

foldr :: (a -> b -> b) -> b -> [a] -> b
foldr _ e []     = e
foldr f e (x:xs) = f x (foldr f e xs)

(.) :: (b -> c) -> (a -> b) -> a -> c
(.) f g x = f (g x)
```
The [map function](../../../../../map-higher-order-function.md) preserves the [list](../../../../../list-abstract-data-type.md) shape while changing element type from `a` to `b`. The [right fold](../../../../../list-fold.md) replaces the empty [list](../../../../../list-abstract-data-type.md) by `e` and each constructor by `f`, whose second argument and result therefore share the accumulator type `b`. [Function composition](../../../../../function-composition.md) requires the output type of `g` to agree with the input type of `f`. No [Haskell type class](../../../../../haskell-type-class.md) constraints arise: these definitions never compare elements or perform arithmetic on them.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

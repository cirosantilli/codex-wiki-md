<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [right fold](../../../../../list-fold.md) definition `xs ++ ys = foldr (:) ys xs`, the right-identity law `xs ++ [] = xs`, and the finite-[list](../../../../../list-abstract-data-type.md) involution law `reverse (reverse xs) = xs`. The last two laws are the additional results used here. Part (b) now gives
```
xs ++ ys
= foldr (:) ys xs
= foldl (flip (:)) ys (reverse xs)
```
Set `ys = []` to obtain `xs = foldl (flip (:)) [] (reverse xs)`. Substitute `reverse xs` for `xs` and simplify the double reversal:
```
reverse xs
= foldl (flip (:)) [] (reverse (reverse xs))
= foldl (flip (:)) [] xs
```
The derived [Haskell](../../../../../haskell.md) definition is therefore
```
reverse :: [a] -> [a]
reverse = foldl (flip (:)) []
```
**Each step prepends the next element to the accumulator.** This is a [left fold](../../../../../left-fold.md) derivation from [list concatenation](../../../../../list-concatenation.md), rather than merely a proposed implementation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

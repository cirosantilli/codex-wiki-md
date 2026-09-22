<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

All three [Haskell](../../../../../haskell.md) definitions have **`filter :: (a -> Bool) -> [a] -> [a]`**. A recursive [list filter](../../../../../list-filter.md) is
```
filter p [] = []
filter p (x:xs)
  | p x       = x : filter p xs
  | otherwise = filter p xs
```
A [list comprehension](../../../../../list-comprehension.md) gives `filter p xs = [x | x <- xs, p x]`. A [right fold](../../../../../list-fold.md) gives
```
filter p = foldr (\x ys -> if p x then x:ys else ys) []
```
Each version retains the input order and needs no [equality](../../../../../equality-mathematics.md) or [Haskell Ord class](../../../../../haskell-ord-class.md) constraint on the element type.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

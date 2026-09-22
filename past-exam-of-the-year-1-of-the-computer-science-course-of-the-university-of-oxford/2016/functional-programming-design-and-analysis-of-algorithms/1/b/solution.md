<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Again use [structural induction](../../../../../structural-induction.md) on the finite [list](../../../../../list-abstract-data-type.md). At `[]`, both the [right fold](../../../../../list-fold.md) and the [left fold](../../../../../left-fold.md) return `e`. For `x:xs`, use `reverse (x:xs) = reverse xs ++ [x]`, part (a), and the definition of `flip`:
```
foldl (flip f) e (reverse (x:xs))
= foldl (flip f) e (reverse xs ++ [x])
= foldl (flip f) (foldl (flip f) e (reverse xs)) [x]
= flip f (foldl (flip f) e (reverse xs)) x
= f x (foldl (flip f) e (reverse xs))
= f x (foldr f e xs)
= foldr f e (x:xs)
```
The penultimate equality uses the [induction hypothesis](../../../../../induction-hypothesis.md). Thus **`foldr f e xs = foldl (flip f) e (reverse xs)`**. Finiteness matters: reversing an infinite [list](../../../../../list-abstract-data-type.md) does not produce its first element, whereas some [right folds](../../../../../list-fold.md) do.

## ↑ Ancestors (12)

1. [B](../b.md)
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

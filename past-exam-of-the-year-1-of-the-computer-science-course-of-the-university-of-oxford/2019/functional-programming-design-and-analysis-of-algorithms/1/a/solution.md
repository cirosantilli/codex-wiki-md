<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [right fold](../../../../../list-fold.md) replaces the two [list](../../../../../list-abstract-data-type.md) constructors by its two arguments; the [left fold](../../../../../left-fold.md) instead updates an accumulator while traversing the [list](../../../../../list-abstract-data-type.md).

```
foldr :: (a -> b -> b) -> b -> [a] -> b
foldr c z []     = z
foldr c z (x:xs) = c x (foldr c z xs)

foldl :: (b -> a -> b) -> b -> [a] -> b
foldl s a []     = a
foldl s a (x:xs) = foldl s (s a x) xs
```

Thus **`foldr` is the natural [list fold](../../../../../list-fold.md)**: it preserves the constructor arrangement while replacing `[]` by `z` and `(:)` by `c`. In particular, `foldr (:) [] = id`. More generally, the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md) says that the defining equations characterize the corresponding [structural recursion](../../../../../structural-recursion.md). Association and [lazy evaluation](../../../../../lazy-evaluation.md) are separate: the accumulator in this definition of [left fold](../../../../../left-fold.md) is not automatically evaluated at each step.[Chapter 9, PreludeList: foldr and foldl](../../../../../haskell-2010-language-report.md)

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Change the [right fold](../../../../../list-fold.md)'s result type to an accumulator-transforming [function type](../../../../../function-type.md):
```
foldlAsFoldr :: (b -> a -> b) -> b -> [a] -> b
foldlAsFoldr s n xs = foldr c id xs n
  where
    c x k a = k (s a x)
```
Thus **`c x k = \a -> k (s a x)` and `k = id`** in the question's notation. Here `c :: a -> (b -> b) -> (b -> b)`, and the fold's base value is the identity [function](../../../../../function-split.md), not the initial accumulator `n`.

The [recursion invariant](../../../../../recursion-invariant.md) is `foldr c id xs a = foldl s a xs` for every `a`. For `[]`, both sides equal `a`. For a cons:
```
foldr c id (x:xs) a
 = c x (foldr c id xs) a
 = foldr c id xs (s a x)
 = foldl s (s a x) xs
 = foldl s a (x:xs).
```
At an undefined spine, applying the undefined folded [function](../../../../../function-split.md) also gives the [bottom value](../../../../../bottom-value.md). The finite-approximation argument then covers infinite [lazy lists](../../../../../lazy-list.md). This is a [continuation representation of a left fold](../../../../../continuation-representation-of-a-left-fold.md): the result retains the operation still to be performed, avoiding the information loss in part (d).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

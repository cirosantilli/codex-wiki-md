<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take **`h = (.)`**:
```
h :: (b -> c) -> (a -> b) -> a -> c
h f g x = f (g x)
```
This is its standalone [principal type](../../../../../principal-type.md); in the [right fold](../../../../../list-fold.md), `c` specializes to the type of a function from the accumulator to itself.

For fixed `f`, `g` and `e`, prove equality pointwise by [structural induction](../../../../../structural-induction.md) on the [list](../../../../../list-abstract-data-type.md). At `[]` both sides return `e`. For `x:xs`, assume the equality for `xs` and calculate:
```
foldr f e (map g (x:xs))
  = f (g x) (foldr f e (map g xs))
  = f (g x) (foldr (h f g) e xs)
  = h f g x (foldr (h f g) e xs)
  = foldr (h f g) e (x:xs)
```
The second equality is the [induction hypothesis](../../../../../induction-hypothesis.md). [Function extensionality](../../../../../function-extensionality.md) gives the required equality of composed functions. This is an instance of the [right-fold fusion law](../../../../../right-fold-fusion-law.md).

For the full lazy [Haskell](../../../../../haskell.md) interpretation, include a [bottom value](../../../../../bottom-value.md) for an undefined list spine: both sides are bottom there. The same constructor argument covers every finite approximation with an undefined tail. The [Scott continuity](../../../../../scott-continuity.md) of the list operations then extends equality to their limits, including infinite [lists](../../../../../list-abstract-data-type.md). Ordinary induction on finite total [lists](../../../../../list-abstract-data-type.md) alone proves only that restricted case.

## ↑ Ancestors (12)

1. [B](../b.md)
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

<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [structural induction](../../../../../structural-induction.md) on the finite [list](../../../../../list-abstract-data-type.md) `xs`, with the assertion quantified over every accumulator `e` and every [list](../../../../../list-abstract-data-type.md) `ys`. The equations of the [left fold](../../../../../left-fold.md) are `foldl f e [] = e` and `foldl f e (x:xs) = foldl f (f e x) xs`.

For `xs = []`, both sides reduce to `foldl f e ys`. For the constructor case, [equational reasoning](../../../../../equational-reasoning.md) gives
```
foldl f e ((x:xs) ++ ys)
= foldl f e (x : (xs ++ ys))
= foldl f (f e x) (xs ++ ys)
= foldl f (foldl f (f e x) xs) ys
= foldl f (foldl f e (x:xs)) ys
```
The third equality uses the [induction hypothesis](../../../../../induction-hypothesis.md) with accumulator `f e x`. Hence **the stated identity holds**. No inspection of `ys` was required: in [Haskell](../../../../../haskell.md) this equality also permits infinite or partially defined `ys`, with both expressions denoting the same possibly undefined result.

## ↑ Ancestors (12)

1. [A](../a.md)
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

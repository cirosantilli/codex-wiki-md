<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The expression parses as `g . (g x)`. Initially write `g :: a -> r` and `x :: a`. In the [function composition](../../../../../function-composition.md), `g x` must itself be a function whose result can be passed to `g`. Hence `r = b -> a` for a fresh type `b`, so
```
g :: a -> b -> a
g x :: b -> a
g . g x :: b -> b -> a
```
Consequently the [principal type](../../../../../principal-type.md) is
```
f :: (a -> b -> a) -> a -> b -> b -> a
```
One can check the constraints by expanding the composition:
```
f g x y z = g (g x y) z
```
Here `g x y` has type `a`, and the second application accepts it and the final `b`-typed argument `z`. The two type variables remain independent; no [Haskell type class](../../../../../haskell-type-class.md) constraints are required.

## ↑ Ancestors (12)

1. [D](../d.md)
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

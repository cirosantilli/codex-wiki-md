<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Application binds more tightly than [function composition](../../../../../function-composition.md), and `(.)` associates to the right. Let

```
g :: a -> b -> c
```

Then `y :: a` and `g y :: b -> c`. To compose to its left, `h x` must have type `c -> a`, so `x :: d` and `h :: d -> c -> a`. The outer occurrence of `g` receives that `a`, producing a function of type `b -> c`. Consequently `g . h x . g y` has type `b -> b -> c`, and the [principal type](../../../../../principal-type.md) is **`f :: (a -> b -> c) -> (d -> c -> a) -> d -> a -> b -> b -> c`**. No [Haskell type class](../../../../../haskell-type-class.md) constraint is introduced.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The most general [polymorphic](../../../../../programming-language-polymorphism.md) [type signatures](../../../../../type-signature.md) and definitions are:

```
infixr 9 .

(.) :: (b -> c) -> (a -> b) -> a -> c
(f . g) x = f (g x)

zipWith :: (a -> b -> c) -> [a] -> [b] -> [c]
zipWith f (x:xs) (y:ys) = f x y : zipWith f xs ys
zipWith _ _ _ = []

uncurry :: (a -> b -> c) -> (a,b) -> c
uncurry f (x,y) = f x y
```

[Function composition](../../../../../function-composition.md) passes the result of the second function into the first. `zipWith` combines corresponding [list](../../../../../list-abstract-data-type.md) elements and stops when either list ends. [Uncurrying](../../../../../uncurrying.md) converts a function taking two successive arguments into one taking a pair. None of these operations needs a numeric or ordering constraint.

## ↑ Ancestors (12)

1. [A](../a.md)
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

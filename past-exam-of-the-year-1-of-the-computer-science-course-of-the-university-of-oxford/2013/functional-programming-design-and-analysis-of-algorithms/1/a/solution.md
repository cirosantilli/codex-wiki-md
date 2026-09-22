<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [map function](../../../../../map-higher-order-function.md) changes each element of a [list](../../../../../list-abstract-data-type.md) while preserving its order and length. [List concatenation](../../../../../list-concatenation.md) removes one level of nesting. [Currying](../../../../../currying.md) changes a [function](../../../../../function-split.md) on a pair into a [function](../../../../../function-split.md) taking its two arguments separately; [uncurrying](../../../../../uncurrying.md) reverses this conversion:

```
map :: (a -> b) -> [a] -> [b]
map f []     = []
map f (x:xs) = f x : map f xs

concat :: [[a]] -> [a]
concat []       = []
concat (xs:xss) = xs ++ concat xss

curry :: ((a, b) -> c) -> a -> b -> c
curry f x y = f (x, y)

uncurry :: (a -> b -> c) -> (a, b) -> c
uncurry f (x, y) = f x y
```

These [polymorphic](../../../../../programming-language-polymorphism.md) [type signatures](../../../../../type-signature.md) impose no numerical, equality or ordering constraints: the definitions only inspect [list](../../../../../list-abstract-data-type.md) or pair structure and apply a supplied [function](../../../../../function-split.md). In particular,

$$
\boxed{\operatorname{curry}(f)\,x\,y=f(x,y),\qquad \operatorname{uncurry}(g)(x,y)=g\,x\,y.}
$$

The recursive equations describe the two possible [list](../../../../../list-abstract-data-type.md) constructors, so they also explain how the empty case terminates each finite computation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

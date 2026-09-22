<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let `x :: a` and `g :: a -> b`, as required by the inner application `g x`. Using `g x` as the next argument of that same `g` forces `b = a`. Thus `g (g x) :: a`. Applying that result to `x` requires a function type `a -> c`, giving

$$
\boxed{a=a\to c.}
$$

This equation fails the [occurs check](../../../../../occurs-check.md): the type variable `a` occurs inside the type with which it would be unified. These constraints have no solution in the [Hindley-Milner type system](../../../../../hindley-milner-type-system.md). Therefore **the definition has no type in ordinary [Haskell](../../../../../haskell.md)**. The obstruction is to [type inference](../../../../../type-inference.md), independently of which particular values might later be supplied.

## ↑ Ancestors (12)

1. [C](../c.md)
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

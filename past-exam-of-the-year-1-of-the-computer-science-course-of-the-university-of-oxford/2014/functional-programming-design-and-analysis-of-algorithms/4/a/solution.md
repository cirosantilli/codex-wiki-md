<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The most general [polymorphic](../../../../../programming-language-polymorphism.md) [type signatures](../../../../../type-signature.md) and recursive definitions are:

```
foldr :: (a -> b -> b) -> b -> [a] -> b
foldr _ z []     = z
foldr f z (x:xs) = f x (foldr f z xs)

infixr 5 ++
(++) :: [a] -> [a] -> [a]
[]     ++ ys = ys
(x:xs) ++ ys = x : (xs ++ ys)

concat :: [[a]] -> [a]
concat []       = []
concat (xs:xss) = xs ++ concat xss
```

The [right fold](../../../../../list-fold.md) replaces constructors by a supplied step and seed; [list concatenation](../../../../../list-concatenation.md) replaces the end of its first argument by its second; flattening concatenates each inner [list](../../../../../list-abstract-data-type.md). In particular,

$$
\boxed{\operatorname{concat}=\operatorname{foldr}(\mathbin{++})[],\qquad xs\mathbin{++}ys=\operatorname{foldr}(:)\ ys\ xs.}
$$

The [right fold](../../../../../list-fold.md) allows different element and accumulator types; the [list concatenation](../../../../../list-concatenation.md) operations require one common element type.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

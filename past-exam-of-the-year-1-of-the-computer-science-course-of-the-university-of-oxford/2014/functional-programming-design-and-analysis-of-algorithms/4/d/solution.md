<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First define argument reversal, with its most general [polymorphic](../../../../../programming-language-polymorphism.md) [type signature](../../../../../type-signature.md):

```
flip :: (a -> b -> c) -> b -> a -> c
flip f y x = f x y
```

Use `concat = foldr (++) []`. In the [right-fold fusion law](../../../../../right-fold-fusion-law.md), choose `f = foldr fn e`, `g = (++)`, `a = []`, `b = e`, and `h = flip (foldr fn)`. The base-image condition follows from `foldr fn e [] = e`; strictness follows because a [right fold](../../../../../list-fold.md) inspects its input spine. Part (c) supplies exactly the compatibility condition:

```
f (xs ++ ys)
  = foldr fn (foldr fn e ys) xs
  = flip (foldr fn) xs (f ys)
  = h xs (f ys)
```

Consequently,

$$
\boxed{\operatorname{foldr}\ fn\ e\circ\operatorname{concat}=\operatorname{foldr}\bigl(\operatorname{flip}(\operatorname{foldr}\ fn)\bigr)\ e.}
$$

The accumulator argument of `foldr fn` comes before the inner [list](../../../../../list-abstract-data-type.md), whereas the outer [right fold](../../../../../list-fold.md) supplies the inner [list](../../../../../list-abstract-data-type.md) first; `flip` reconciles those orders. The proof uses fusion and the already proved concatenation identity, without a further [induction](../../../../../mathematical-induction.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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

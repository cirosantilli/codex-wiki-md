<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix `ys` and instantiate the [right-fold fusion law](../../../../../right-fold-fusion-law.md) with

```
f = foldr fn e
g = (:)
a = ys
h = fn
b = foldr fn e ys
```

The [right fold](../../../../../list-fold.md) is a [strict function](../../../../../strict-function.md) of its [list](../../../../../list-abstract-data-type.md) argument. The base-image condition is immediate. For compatibility, expand one constructor:

```
f (x:y) = foldr fn e (x:y)
        = fn x (foldr fn e y)
        = h x (f y)
```

Fusion gives `foldr fn e . foldr (:) ys = foldr fn (foldr fn e ys)`. Apply both sides to `xs` and replace `foldr (:) ys xs` by `xs ++ ys`:

$$
\boxed{\operatorname{foldr}\ fn\ e\ (xs\mathbin{++}ys)=\operatorname{foldr}\ fn\ (\operatorname{foldr}\ fn\ e\ ys)\ xs.}
$$

This is a direct application of the [right-fold fusion law](../../../../../right-fold-fusion-law.md), with no new [induction](../../../../../mathematical-induction.md) proof. It also covers partial and infinite [lists](../../../../../list-abstract-data-type.md) under the semantics established in part (b).

## ↑ Ancestors (12)

1. [C](../c.md)
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

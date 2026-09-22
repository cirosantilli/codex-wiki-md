<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Both uses of `x` in this definition have the same [monomorphic type](../../../../../../monomorphic-type.md) within the body. Write `x :: u -> v`. The inner application `x z` forces `z :: u` and has type `v`; the outer application `x (x z)` forces `v = u`. Thus `x :: u -> u`. Finally, `x (x z)` is applied to `y`, so `u` must itself be a [function type](../../../../../../function-type.md), say `a -> b`. This gives

```
f :: ((a -> b) -> a -> b) -> a -> (a -> b) -> b
f x y z = x (x z) y
```

The [principal type](../../../../../../principal-type.md) is therefore

$$
\boxed{((\alpha\to\beta)\to(\alpha\to\beta))\to\alpha\to(\alpha\to\beta)\to\beta.}
$$

The argument `x` transforms a [function](../../../../../../function-split.md) into another [function](../../../../../../function-split.md) of the same type. The body transforms `z` twice, then applies the resulting [function](../../../../../../function-split.md) to `y`; no recursive type equation is required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

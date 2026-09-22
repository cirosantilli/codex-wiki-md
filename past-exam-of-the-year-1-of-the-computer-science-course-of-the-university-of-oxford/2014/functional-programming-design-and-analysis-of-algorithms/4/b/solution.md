<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For finite [lists](../../../../../list-abstract-data-type.md), prove the [right-fold fusion law](../../../../../right-fold-fusion-law.md) by [structural induction](../../../../../structural-induction.md). The empty case uses the base-image premise:

```
f (foldr g a []) = f a = b = foldr h b []
```

For the cons case, use the compatibility premise, then the [induction hypothesis](../../../../../induction-hypothesis.md):

```
f (foldr g a (x:xs))
  = f (g x (foldr g a xs))
  = h x (f (foldr g a xs))
  = h x (foldr h b xs)
  = foldr h b (x:xs)
```

The assumption that `f` is a [strict function](../../../../../strict-function.md) addresses partial spines. Write $\bot$ for the [bottom value](../../../../../bottom-value.md). A [right fold](../../../../../list-fold.md) must inspect the outer [list](../../../../../list-abstract-data-type.md) constructor, so

$$
f(\operatorname{foldr}\ g\ a\ \bot)=f(\bot)=\bot=\operatorname{foldr}\ h\ b\ \bot.
$$

The same cons calculation therefore establishes equality for finite partial spines ending in $\bot$, including partial heads, because compatibility was assumed for all arguments.

For pure definable [Haskell](../../../../../haskell.md) functions, the results on an infinite [lazy list](../../../../../lazy-list.md) are determined by their results on increasing finite partial approximations. Equality passes to that limit, as formalized by [structural induction on lazy lists](../../../../../structural-induction-on-lazy-lists.md). Thus

$$
\boxed{f\circ\operatorname{foldr}(g,a)=\operatorname{foldr}(h,b).}
$$

For finite total inputs alone, the empty and cons cases suffice. Strictness is needed to extend the claim to undefined spines; the finite-total proof by itself does not justify the infinite-input claim.

## ↑ Ancestors (12)

1. [B](../b.md)
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

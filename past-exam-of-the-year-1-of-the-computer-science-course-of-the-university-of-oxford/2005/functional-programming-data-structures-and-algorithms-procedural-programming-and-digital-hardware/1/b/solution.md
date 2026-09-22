<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P(zss)$ mean `concat (map f zss) = f (concat zss)`. We use [structural induction on lazy lists](../../../../../structural-induction-on-lazy-lists.md), including the [bottom value](../../../../../bottom-value.md) and allowing arbitrary, possibly partial, inner [lists](../../../../../list-abstract-data-type.md).

For `[]`, the left side is `[]` and the right side is `f [] = []`. For the [bottom value](../../../../../bottom-value.md) $\bot$, both `map f` and `concat` are [strict functions](../../../../../strict-function.md) in the outer spine, and the supplied strictness of $f$ makes the right side $f\,\bot=\bot$ too.

For the cons case, assume $P(zss)$ and write the new head as `xs`. The defining equations and the [induction hypothesis](../../../../../induction-hypothesis.md) give

$$
\begin{aligned}
\operatorname{concat}(\operatorname{map}f\,(xs:zss))
&=f(xs)\mathbin{++}\operatorname{concat}(\operatorname{map}f\,zss)\\
&=f(xs)\mathbin{++}f(\operatorname{concat}zss)\\
&=f(xs\mathbin{++}\operatorname{concat}zss)\\
&=f(\operatorname{concat}(xs:zss)).
\end{aligned}
$$

The third equality is exactly the supplied [list concatenation](../../../../../list-concatenation.md) preservation law. No inspection of `xs` was required, so the argument includes partial inner [lists](../../../../../list-abstract-data-type.md) and undefined elements.

This proves the identity for every finite outer spine ending in either `[]` or $\bot$. In the usual pure [Haskell](../../../../../haskell.md) semantics, these [functions](../../../../../function-split.md) are [Scott continuous maps](../../../../../scott-continuity.md). An infinite outer [list](../../../../../list-abstract-data-type.md) is obtained as a limit by [finite approximation of a lazy list](../../../../../finite-approximation-of-a-lazy-list.md); both composite [functions](../../../../../function-split.md) preserve that limit. Equality on all its finite approximations therefore gives equality on the infinite outer [list](../../../../../list-abstract-data-type.md). Equivalently, $P$ is an [admissible predicate on lazy lists](../../../../../admissible-predicate-on-lazy-lists.md). Consequently

$$
\boxed{\operatorname{concat}\circ\operatorname{map}f=f\circ\operatorname{concat}.}
$$

The continuity assumption is the usual semantic assumption for definable [functions](../../../../../function-split.md) here; an extension from finite to infinite inputs cannot be justified by ordinary finite [induction](../../../../../mathematical-induction.md) alone.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

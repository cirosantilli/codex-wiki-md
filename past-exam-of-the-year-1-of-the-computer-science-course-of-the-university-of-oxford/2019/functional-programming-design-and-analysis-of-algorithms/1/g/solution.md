<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Fix `s` and put $R(xs,a)=\mathrm{foldr}\ (k\ s)\ \mathrm{id}\ xs\ a$. The [right fold](../../../../../list-fold.md) equations give

$$
R([],a)=a,\qquad R(x:xs,a)=R(xs,s\ a\ x).
$$

These are exactly the [left fold](../../../../../left-fold.md) equations. [Structural induction](../../../../../structural-induction.md), with the induction hypothesis quantified over _all_ accumulators, proves equality on finite terminating [lists](../../../../../list-abstract-data-type.md).

To include the other input spines, first observe that both applied expressions give $\bot$ on an undefined spine. The same induction proves equality on every finite prefix ending in $\bot$: the step `k s x f a` demands the continuation `f` when its result is demanded. Finally use that the two applied operations are [Scott continuous maps](../../../../../scott-continuity.md), taking the limit over prefixes interpreted as a [finite approximation of a lazy list](../../../../../finite-approximation-of-a-lazy-list.md). This covers infinite spines, on which both applied expressions are $\bot$, and proves the identity for all [lists](../../../../../list-abstract-data-type.md) under the stated [Haskell](../../../../../haskell.md) semantics. The intermediate [right fold](../../../../../list-fold.md) builds an accumulator-transforming [function](../../../../../function-split.md); it does not provide a terminating [left fold](../../../../../left-fold.md) of an infinite [list](../../../../../list-abstract-data-type.md).

## ↑ Ancestors (12)

1. [G](../g.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

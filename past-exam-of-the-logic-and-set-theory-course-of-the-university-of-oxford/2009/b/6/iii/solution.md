<h1 id="b/6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $X$ is finite and nonempty, let $n=|X|\geq1$, choose a [bijection](../../../../../bijection.md) with the [cyclic group](../../../../../cyclic-group.md) $\mathbb Z/n\mathbb Z$, and transport its addition to $X$. This includes the one-element case.

If $X$ is infinite, use the maximal partial [group](../../../../../group-split.md) $(A,m)$ from the preceding part. Its carrier must be infinite: otherwise $|X\setminus A|<|A|$ would make the complement finite too, forcing $X$ finite. Since the complement injects into $A$,

$$
|A|\leq|X|=|A|+|X\setminus A|\leq|A|+|A|=2|A|=|A|,
$$

where the last equality is the permitted infinite-cardinal doubling identity. Cantor-Schröder-Bernstein supplies a [bijection](../../../../../bijection.md) $j:X\to A$. Define

$$
\boxed{x\star y=j^{-1}(m(j(x),j(y))).}
$$

[Associativity](../../../../../associative-property.md) follows by applying $j$ and using [associativity](../../../../../associative-property.md) of $m$; the identity is $j^{-1}(e_A)$ and the inverse of $x$ is $j^{-1}(j(x)^{-1})$. Hence $(X,\star)$ is a [group](../../../../../group-split.md).

This final transport need not extend the earlier partial operation on its original [subset](../../../../../subset.md). That stronger claim is neither needed nor generally possible: for example a [group](../../../../../group-split.md) of order three cannot occur as a [subgroup](../../../../../subgroup.md) of a [group](../../../../../group-split.md) of order four. The proof establishes exactly the existence of some [group structure on every nonempty set](../../../../../group-structure-on-every-nonempty-set.md), using the allowed choice consequences in the infinite case.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

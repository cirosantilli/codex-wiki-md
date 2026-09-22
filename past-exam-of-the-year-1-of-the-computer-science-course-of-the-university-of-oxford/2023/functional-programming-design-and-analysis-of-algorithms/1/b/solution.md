<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [list fold](../../../../../list-fold.md) criterion is: there must be a value `z` and a definable combining function `c` such that

$$
f(\bot)=\bot,\qquad f([])=z,\qquad f(x:xs)=c\ x\ (f\ xs).
$$

The last equality says that all information needed about the tail factors through `f xs`; the combining function receives no other access to `xs`. These conditions give **`f = foldr c z`**.

Necessity follows from the defining equations of `foldr`, including its case distinction on the input [list](../../../../../list-abstract-data-type.md). Sufficiency follows by [structural induction](../../../../../structural-induction.md) for finite lists and finite partial-list approximations. For infinite or partial [lazy lists](../../../../../lazy-list.md), the usual continuous semantics of these definable functions extends equality from the approximations to their limit. The strictness condition matters: agreement only on finite total lists does not establish agreement at $\bot$. This is the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

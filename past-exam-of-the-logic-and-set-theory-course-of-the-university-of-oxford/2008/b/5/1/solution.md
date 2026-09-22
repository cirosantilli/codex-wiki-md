<h1 id="b/5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

First give the recursive definitions, keeping the right argument as the recursion [variable](../../../../../variable-mathematics.md). For [ordinals](../../../../../ordinal-split.md) $\alpha,\beta$ and nonzero [limit ordinals](../../../../../limit-ordinal.md) $\lambda$,

$$
\alpha+0=\alpha,\qquad \alpha+(\beta+1)=(\alpha+\beta)+1,\qquad
\alpha+\lambda=\sup_{\xi<\lambda}(\alpha+\xi),
$$



$$
\alpha\cdot0=0,\qquad \alpha\cdot(\beta+1)=\alpha\beta+\alpha,\qquad
\alpha\lambda=\sup_{\xi<\lambda}\alpha\xi.
$$

Here $\xi+1$ is the [successor ordinal](../../../../../successor-ordinal.md), and the [supremum](../../../../../supremum.md) of a [set](../../../../../set-split.md) of [ordinals](../../../../../ordinal-split.md) is its [union](../../../../../set-union.md). These are [ordinal arithmetic](../../../../../ordinal-arithmetic.md), defined by [transfinite recursion](../../../../../transfinite-recursion.md), and differ from [cardinal sum](../../../../../cardinal-sum.md) and [ordinal multiplication](../../../../../ordinal-multiplication.md).

**[Associativity](../../../../../associative-property.md) of [ordinal addition](../../../../../ordinal-addition.md) is true.** Fix $\alpha,\beta$ and use [transfinite induction](../../../../../transfinite-induction.md) on $\gamma$. The case $\gamma=0$ is immediate. In the successor step the recursive definitions and the induction hypothesis give

$$
(\alpha+\beta)+(\gamma+1)=((\alpha+\beta)+\gamma)+1
=(\alpha+(\beta+\gamma))+1=\alpha+(\beta+(\gamma+1)).
$$

For a nonzero [limit ordinal](../../../../../limit-ordinal.md) $\lambda$, the [ordinals](../../../../../ordinal-split.md) $\beta+\xi$ for $\xi<\lambda$ form an increasing [cofinal subset](../../../../../cofinal-subset.md) of the [limit ordinal](../../../../../limit-ordinal.md) $\beta+\lambda$. The limit clause for [ordinal addition](../../../../../ordinal-addition.md), restricted to this [cofinal subset](../../../../../cofinal-subset.md), gives

$$
(\alpha+\beta)+\lambda
=\sup_{\xi<\lambda}((\alpha+\beta)+\xi)
=\sup_{\xi<\lambda}(\alpha+(\beta+\xi))
=\alpha+(\beta+\lambda).
$$

[Cofinal](../../../../../cofinal-subset.md) restriction is valid because [ordinal addition](../../../../../ordinal-addition.md) by a fixed [ordinal](../../../../../ordinal-split.md) on the left is increasing and continuous in its right argument, directly from its recursive definition. This completes the induction.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

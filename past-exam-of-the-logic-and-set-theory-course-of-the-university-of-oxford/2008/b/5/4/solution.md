<h1 id="b/5/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**True: [ordinal multiplication](../../../../../ordinal-multiplication.md) on the left distributes over [ordinal addition](../../../../../ordinal-addition.md).** If $\alpha=0$ both sides are zero. Otherwise fix $\alpha>0$ and $\beta$, and induct on $\gamma$. At zero the identity follows from $\alpha0=0$. At a successor, use the recursive [ordinal multiplication](../../../../../ordinal-multiplication.md) rule and the [associativity](../../../../../associative-property.md) just proved:

$$
\alpha(\beta+(\gamma+1))
=\alpha((\beta+\gamma)+1)
=\alpha(\beta+\gamma)+\alpha
=(\alpha\beta+\alpha\gamma)+\alpha
=\alpha\beta+\alpha(\gamma+1).
$$

For a nonzero [limit ordinal](../../../../../limit-ordinal.md) $\lambda$, the [ordinals](../../../../../ordinal-split.md) $\beta+\xi$ are [cofinal](../../../../../cofinal-subset.md) in $\beta+\lambda$. [Continuity](../../../../../continuous-function.md) of [ordinal multiplication](../../../../../ordinal-multiplication.md) in its right argument gives

$$
\alpha(\beta+\lambda)
=\sup_{\xi<\lambda}\alpha(\beta+\xi)
=\sup_{\xi<\lambda}(\alpha\beta+\alpha\xi)
=\alpha\beta+\alpha\lambda.
$$

For the last [equality](../../../../../equality-mathematics.md), $\alpha\xi$ is increasing and [cofinal](../../../../../cofinal-subset.md) in $\alpha\lambda$, which is a [limit ordinal](../../../../../limit-ordinal.md) because $\alpha>0$, and [ordinal addition](../../../../../ordinal-addition.md) is continuous in its right argument. This establishes the limit step and the identity for all [ordinals](../../../../../ordinal-split.md).

## ↑ Ancestors (13)

1. [4](../4.md)
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

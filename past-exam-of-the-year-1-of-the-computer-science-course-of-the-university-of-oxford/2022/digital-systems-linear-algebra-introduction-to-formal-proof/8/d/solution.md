<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the intended [first-order structure](../../../../../first-order-structure.md) of real arithmetic, with `Int` selecting the [integers](../../../../../integer-split.md); $z$ is the parameter in $\phi_z$. A suitable [first-order formula](../../../../../first-order-formula.md) is

$$
\boxed{\phi_z=\exists r\left(r*r=(1+1)*z\ \land\ \neg\exists p\,\exists q\left(\operatorname{Int}(p)\land\operatorname{Int}(q)\land\neg(q=0)\land q*r=p\right)\right).}
$$

The first condition requires a real [square root](../../../../../square-root.md) of $2z$. The second excludes every representation as a [rational number](../../../../../rational-number.md) $p/q$ with a nonzero [integer](../../../../../integer-split.md) denominator. This uses only the listed function and constant symbols, the `Int` predicate and [logical equality](../../../../../logical-equality.md); in particular, $2$ is written $1+1$ and there is no extra division symbol. A [square root](../../../../../square-root.md) exists exactly when $z\ge0$, and either sign of a root is a [rational number](../../../../../rational-number.md) exactly when the other sign is a [rational number](../../../../../rational-number.md), so the absence of a positivity condition on $r$ does not affect the claim about the principal [square root](../../../../../square-root.md). At $z=0$ the formula is false; for $z<0$ there is no real witness. The meanings of $+$ and $*$ as real arithmetic, not just the meaning of `Int`, are part of this interpretation.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

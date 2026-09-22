<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the additive zero singleton, $x+x=x$ is already a [quantifier-free formula](../../../../../quantifier-free-formula.md), so it is also an [existential formula](../../../../../existential-formula.md) and a [universal formula](../../../../../universal-formula.md) with an empty quantifier block. If a nonempty block is required, add a dummy $\exists y$ or $\forall y$; first-order domains are nonempty.

For the two definable multiplicative singletons, [existential formulas](../../../../../existential-formula.md) are

$$
\boxed{\begin{aligned}
0:\quad&\exists y\,(x\cdot x=x\ \land\ x\cdot y\ne y),\\
1:\quad&\exists y\,(x\cdot x=x\ \land\ x\cdot y\ne x).
\end{aligned}}
$$

In the integers, the equation $x^2=x$ restricts $x$ to zero or one. In the first line, one never satisfies the inequality, whereas zero does with $y=1$. In the second, zero never satisfies it, whereas one does with $y=0$. The respective [universal formulas](../../../../../universal-formula.md) are $\forall y(xy=x)$ and $\forall y(xy=y)$, as already verified.

Neither multiplicative singleton has a [quantifier-free formula](../../../../../quantifier-free-formula.md). In this constant-free, multiplication-only language, every term in the sole free variable $x$ is $x^k$ for a positive integer $k$. Every [atomic formula](../../../../../atomic-formula.md) $x^r=x^s$ is true at both zero and one. Every Boolean combination consequently has the same truth value at those two points, and cannot separate their singletons. This is the fact that [zero and one have the same quantifier-free type in the multiplicative integers](../../../../../zero-and-one-have-the-same-quantifier-free-type-in-the-multiplicative-integers.md).

Thus **additive zero admits all three forms; multiplicative zero and one admit existential and universal forms, but no quantifier-free form**. All remaining cases were excluded from definability itself by [structure automorphisms](../../../../../automorphism-of-a-first-order-structure.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the model theory course of the University of Oxford](../../../../split.md)
6. [Model theory course of the University of Oxford](../../../../../model-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

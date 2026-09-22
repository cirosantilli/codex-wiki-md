<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [regular perturbation](../../../../../../regular-perturbation.md) admits an [asymptotic expansion](../../../../../../asymptotic-expansion.md) about the limiting problem on the relevant scale without losing its solutions or conditions. A [singular perturbation](../../../../../../singular-perturbation.md) changes the limiting structure, so some solutions require a different scale: a differential equation may lose an order, or a [polynomial](../../../../../../polynomial-split.md) may lose its degree.

The two finite roots approach $s=\pm\sqrt2$. Set $x=s+\epsilon a+O(\epsilon^2)$. Substitution into the [polynomial](../../../../../../polynomial-split.md) gives $s^2-2=0$ at leading order and $s^3+2sa=0$ at the next order. Since $s^2=2$, $a=-1$ for either sign. Each branch is a [regular perturbation of a simple algebraic root](../../../../../../regular-perturbation-of-a-simple-algebraic-root.md), with

$$
\boxed{x_+=\sqrt2-\epsilon+O(\epsilon^2),\qquad x_-=-\sqrt2-\epsilon+O(\epsilon^2).}
$$

The limiting quadratic has only two roots, whereas the original equation has three. The missing root is a [divergent algebraic root in a singular perturbation](../../../../../../divergent-algebraic-root-in-a-singular-perturbation.md). The [dominant balance for algebraic roots](../../../../../../dominant-balance-for-algebraic-roots.md) sets $x=\epsilon^{-1}X$, giving $X^3+X^2=2\epsilon^2$. Its nonzero leading root is $X=-1$. Put $X=-1+a\epsilon^2+O(\epsilon^4)$; the left side is $a\epsilon^2+O(\epsilon^4)$, so $a=2$. Hence the second nonzero term occurs at order $\epsilon$, not order one:

$$
\boxed{x_3=-\epsilon^{-1}+2\epsilon+O(\epsilon^3).}
$$

For small nonzero real $\epsilon$ these three branches are real and distinct; the divergent branch changes sign with $\epsilon$. The two bounded branches are regular even though the full root problem is singular.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

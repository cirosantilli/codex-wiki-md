<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The limiting [polynomial](../../../../../../polynomial-split.md) has a [double root](../../../../../../double-root.md) at $x=-1$, so two roots require a [Puiseux series](../../../../../../puiseux-series.md). For positive $\epsilon$, put $\delta=\sqrt\epsilon$ and $x=-1+a\delta+b\delta^2+\cdots$. Substitution and [dominant balance](../../../../../../dominant-balance.md) give

$$
0=(a^2-1)\delta^2+(2ab+3a)\delta^3+O(\delta^4).
$$

Thus $a=\pm1$ and $b=-3/2$. The two finite roots have the three-term [asymptotic expansions](../../../../../../asymptotic-expansion.md)

$$
\boxed{x_\pm=-1\pm\epsilon^{1/2}-\frac32\epsilon+O(\epsilon^{3/2}).}
$$

This is [square-root splitting of a double polynomial root](../../../../../../square-root-splitting-of-a-double-polynomial-root.md). For negative $\epsilon$, the same formulas apply with a chosen complex square root and describe a [complex conjugate](../../../../../../complex-conjugate.md) pair.

The third root is a [divergent algebraic root in a singular perturbation](../../../../../../divergent-algebraic-root-in-a-singular-perturbation.md). Set $x=X/\epsilon$: the equation for $X$ is $X^3+X^2+2\epsilon X+\epsilon^2=0$. Its nonzero limiting root is $X=-1$. Substituting $X=-1+A\epsilon+B\epsilon^2+\cdots$ yields $A=2$ and $B=3$, hence

$$
\boxed{x_L=-\epsilon^{-1}+2+3\epsilon+O(\epsilon^2).}
$$

As an independent check, [Vieta formulas](../../../../../../vieta-formulas.md) give the sum of roots as $-1/\epsilon$: the two finite-root expansions sum to $-2-3\epsilon+O(\epsilon^2)$, giving the same large-root expansion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

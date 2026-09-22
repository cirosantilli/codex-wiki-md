<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\Re s>1$, the [Riemann zeta function](../../../../../../riemann-zeta-function.md) is the [absolutely convergent](../../../../../../absolute-convergence.md) [Dirichlet series](../../../../../../dirichlet-series.md) $\zeta(s)=\sum_{n\ge1}n^{-s}$. Apply [Abel summation](../../../../../../abel-s-summation-formula.md) to the tail, with counting function $\lfloor w\rfloor-\lfloor x\rfloor$. The upper boundary term tends to zero, giving

$$
\sum_{n>x}n^{-s}=-\lfloor x\rfloor x^{-s}+s\int_x^\infty\lfloor w\rfloor w^{-s-1}\,dw.
$$

Substitute $\lfloor w\rfloor=w-\{w\}$ and integrate the $w$ term. This proves the [fractional-part continuation formula for the Riemann zeta function](../../../../../../fractional-part-continuation-formula-for-the-riemann-zeta-function.md)

$$
\boxed{\zeta(s)=\sum_{n\le x}n^{-s}+\frac{x^{1-s}}{s-1}+\{x\}x^{-s}-s\int_x^\infty\{w\}w^{-s-1}\,dw.}
$$

The endpoint convention is valid whether or not $x$ is an integer. Since $0\le\{w\}<1$, the last integral converges locally uniformly for $\Re s>0$, including after differentiation on compact subsets. It therefore defines a [holomorphic function](../../../../../../holomorphic-function.md) there. The other terms are entire except for $x^{1-s}/(s-1)$. By the [identity theorem for holomorphic functions](../../../../../../identity-theorem.md), the formula supplies a [meromorphic continuation](../../../../../../meromorphic-continuation.md) with **exactly one [pole](../../../../../../pole.md) in $\Re s>0$: a simple [pole](../../../../../../pole.md) at $s=1$ of [residue](../../../../../../residue.md) one.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

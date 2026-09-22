<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\Re s>1$, the absolutely convergent [Dirichlet series](../../../../../../dirichlet-series.md)

$$
\zeta(s)=\sum_{n=1}^\infty n^{-s}
$$

defines the [Riemann zeta function](../../../../../../riemann-zeta-function.md). To continue it, use [partial summation](../../../../../../abel-s-summation-formula.md) in Stieltjes form:

$$
\zeta(s)
=s\int_1^\infty\lfloor x\rfloor x^{-s-1}\,dx
=\frac{s}{s-1}-s\int_1^\infty\{x\}x^{-s-1}\,dx.
$$

Since $0\leq\{x\}<1$, the final integral converges locally uniformly for $\Re s>0$ and is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) there. The displayed expression is consequently a [meromorphic function](../../../../../../meromorphic-function.md) on that half-plane, with its only pole at $s=1$. Since $s/(s-1)$ has residue one there, so does $\zeta$. Agreement in $\Re s>1$ makes this continuation unique by the [identity theorem](../../../../../../identity-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

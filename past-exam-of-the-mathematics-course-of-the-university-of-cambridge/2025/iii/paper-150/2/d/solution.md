<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put

$$
A(x)=\sum_{n\leq x}\Lambda(n)n^{iu}
=\frac{x^{1+iu}}{1+iu}+O\left(x^{1/2}(\log x)^2\right).
$$

For $\Re s>1$, [partial summation](../../../../../../abel-s-summation-formula.md) gives

$$
-\frac{\zeta'(s-iu)}{\zeta(s-iu)}
=s\int_1^\infty A(x)x^{-s-1}\,dx
=\frac{s}{(1+iu)(s-1-iu)}
+s\int_1^\infty O\left(x^{1/2}(\log x)^2\right)x^{-s-1}\,dx.
$$

The last integral is holomorphic for $\Re s>1/2$. Thus the logarithmic derivative on the left continues meromorphically to that half-plane with no pole except $s=1+iu$.

A zero $\rho$ of $\zeta$ with $\Re\rho>1/2$ would make $-\zeta'(s-iu)/\zeta(s-iu)$ singular at $s=\rho+iu$, a contradiction unless $\rho=1$, which is a pole rather than a zero. Therefore no nontrivial zero lies to the right of the [critical line](../../../../../../critical-line.md). The [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md) reflects zeros across that line, so none lies to its left either. Every nontrivial zero lies on the critical line, proving the [Riemann hypothesis](../../../../../../riemann-hypothesis.md). This is the [Twisted Von Mangoldt estimate implying the Riemann hypothesis](../../../../../../twisted-von-mangoldt-estimate-implying-the-riemann-hypothesis.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

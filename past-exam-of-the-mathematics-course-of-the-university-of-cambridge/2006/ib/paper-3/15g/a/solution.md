<h1 id="15g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Fourier sine series](../../../../../../fourier-sine-series.md) on $(0,1)$, [orthogonality](../../../../../../orthogonal-vectors.md) gives

$$
b_n=2\int_0^1x\sin(n\pi x)\,dx
=2\left[-\frac{x\cos(n\pi x)}{n\pi}+\frac{\sin(n\pi x)}{n^2\pi^2}\right]_0^1
=\frac{2(-1)^{n+1}}{n\pi}.
$$

Therefore

$$
\boxed{x=\sum_{n=1}^{\infty}\frac{2(-1)^{n+1}}{n\pi}\sin(n\pi x),\qquad 0<x<1.}
$$

The series is that of the odd, two-periodic extension. At $x=0$ its value is zero, agreeing with $f(0)$; at $x=1$ every summand is zero and the series converges to zero, the average of the two one-sided extension limits. Thus it represents the function in the interior and in the square-integrable sense, **not the prescribed value one at the endpoint $x=1$**. This endpoint issue matters when using sine expansions with homogeneous boundary conditions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15G](../../15g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

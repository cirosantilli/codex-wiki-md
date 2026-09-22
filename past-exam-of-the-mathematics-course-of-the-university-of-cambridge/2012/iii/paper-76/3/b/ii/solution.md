<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The real-space expression $1/x$ means the [principal-value reciprocal distribution](../../../../../../../principal-value-reciprocal-distribution.md). Apply even exponential damping. Oddness gives

$$
\widehat{e^{-a|x|}\operatorname{PV}(1/x)}(k)=-2i\int_0^\infty e^{-ax}\frac{\sin(kx)}x\,dx.
$$

Differentiate the integral with respect to $k$; its derivative is $\int_0^\infty e^{-ax}\cos(kx)dx=a/(a^2+k^2)$. Its value at $k=0$ is zero, so the integral equals $\arctan(k/a)$. Taking $a\downarrow0$ gives

$$
\boxed{\widehat{\operatorname{PV}(1/x)}(k)=-i\pi\operatorname{sgn}k.}
$$

The limit is a [tempered distribution](../../../../../../../tempered-distribution.md) limit: the regularized transforms are uniformly bounded and converge away from zero, allowing dominated convergence against a [Schwartz function](../../../../../../../schwartz-function.md). This [Fourier transform of a principal-value reciprocal](../../../../../../../principal-value-fourier-transform-of-a-real-pole.md) argument also establishes the needed Dirichlet integral $\int_0^\infty\sin u/u\,du=\pi/2$ in its Abel interpretation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

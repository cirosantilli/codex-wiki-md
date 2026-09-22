<h1 id="17d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Evaluate the absolutely convergent [complex Fourier series](../../../../../../complex-fourier-series.md) at $x=\pi$. The factors $(-1)^ne^{in\pi}$ equal one, and the $n=0$ term is $1/\alpha^2$. Pairing positive and negative integers gives

$$
 \cos(\pi\alpha)=\frac{\alpha\sin(\pi\alpha)}\pi
 \left[\frac1{\alpha^2}-2\sum_{n=1}^\infty\frac1{n^2-\alpha^2}\right].
$$

Since $\sin(\pi\alpha)\ne0$ for nonintegral complex $\alpha$, rearranging proves

$$
 \boxed{\sum_{n=1}^\infty\frac1{n^2-\alpha^2}
 =\frac1{2\alpha^2}-\frac{\pi}{2\alpha\tan(\pi\alpha)}.}
$$

The last term means $\pi\cot(\pi\alpha)/(2\alpha)$, so half-integer arguments are included by the finite cotangent value zero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [17D](../../17d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because the function is [even](../../../../../even-function.md), all sine [Fourier coefficients](../../../../../fourier-coefficient.md) vanish. Its average is zero, so $a_0=0$. The [Fourier cosine coefficients of a sine mode](../../../../../fourier-cosine-coefficients-of-a-sine-mode.md) follow from the product-to-sum identity:

$$
a_n=\frac2\pi\int_0^\pi\sin2x\cos nx\,dx=\begin{cases}\displaystyle\frac8{\pi(4-n^2)},&n\text{ odd},\\0,&n\text{ even}.\end{cases}
$$

For $n=2$, the integral is directly zero rather than an undefined substitution into a denominator. Thus

$$
\boxed{f(x)=\frac8\pi\sum_{m=0}^\infty\frac{\cos((2m+1)x)}{4-(2m+1)^2}.}
$$

The [Fourier series](../../../../../fourier-series-split.md) equals the continuous function at every point, including the corners. Its coefficients decay quadratically, so the series is also [absolutely convergent](../../../../../absolute-convergence.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

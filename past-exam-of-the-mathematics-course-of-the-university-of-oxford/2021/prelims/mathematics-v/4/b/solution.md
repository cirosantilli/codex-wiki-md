<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For period two, write $f\sim a_0/2+\sum_{n\geq1}[a_n\cos(n\pi x)+b_n\sin(n\pi x)]$. Direct integration gives $a_0=1/2$. For $0<x<1$, $f(x)+f(-x)=2-3x$ and $f(x)-f(-x)=x$, so

$$
a_n=\int_0^1(2-3x)\cos(n\pi x)\,dx=\frac{3(1-(-1)^n)}{n^2\pi^2},\qquad
b_n=\int_0^1x\sin(n\pi x)\,dx=\frac{(-1)^{n+1}}{n\pi}.
$$

Thus the [Fourier series](../../../../../../fourier-series-split.md) is

$$
\boxed{\frac14+\sum_{n=1}^\infty\left[
\frac{3(1-(-1)^n)}{n^2\pi^2}\cos(n\pi x)+\frac{(-1)^{n+1}}{n\pi}\sin(n\pi x)\right].}
$$

It converges to the values specified in part [a](../a.md). Changing the assigned values at the jumps would not change these [integral](../../../../../../integral-split.md) coefficients.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

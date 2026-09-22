<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [tempered distribution](../../../../../tempered-distribution.md) is a continuous [linear functional](../../../../../linear-functional.md) $u:\mathcal S(\mathbb R)\to\mathbb C$. Equivalently, for some integer $N$ and constant $C$,

$$
|\langle u,\phi\rangle|\leq C\sum_{0\leq m,n\leq N}p_{m,n}(\phi)
\qquad(\phi\in\mathcal S(\mathbb R)).
$$

The [Fourier transform of a tempered distribution](../../../../../fourier-transform-of-a-tempered-distribution.md) is defined by

$$
\boxed{\langle\widehat u,\phi\rangle:=\langle u,\widehat\phi\rangle.}
$$

The [Fourier bounds for Schwartz functions](../../../../../fourier-bounds-for-schwartz-functions.md) make the right side a continuous [linear functional](../../../../../linear-functional.md) on the [Schwartz space](../../../../../schwartz-space.md), so $\widehat u$ is again a [tempered distribution](../../../../../tempered-distribution.md).

For an [integrable function](../../../../../lebesgue-integrable-function.md) $f$, the [regular distribution](../../../../../regular-distribution.md) $u_f$ acts by $\langle u_f,\phi\rangle=\int f\phi$. The estimate $|\langle u_f,\phi\rangle|\leq\|f\|_1p_{0,0}(\phi)$ proves it is a [tempered distribution](../../../../../tempered-distribution.md). Since $\iint|f(x)\phi(\xi)|\,dx\,d\xi<\infty$, [Fubini's theorem](../../../../../fubini-s-theorem.md) gives

$$
\langle\widehat{u_f},\phi\rangle
=\int f(x)\int\phi(\xi)e^{-ix\xi}\,d\xi\,dx
=\int\widehat f(\xi)\phi(\xi)\,d\xi
=\langle u_{\widehat f},\phi\rangle.
$$

Thus the [distributional Fourier transform](../../../../../fourier-transform-of-a-tempered-distribution.md) agrees with the ordinary [Fourier transform](../../../../../fourier-transform-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

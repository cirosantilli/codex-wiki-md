<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $s=\omega t$, so the nonzero half-cycle is $0\leq s\leq\pi$. The constant coefficient is

$$
a_0=\frac{V_0}{\pi}\int_0^\pi\sin s\,ds=\frac{2V_0}{\pi}.
$$

The [sine](../../../../../sine.md) coefficients satisfy

$$
b_n=\frac{V_0}{\pi}\int_0^\pi\sin s\sin ns\,ds
=\begin{cases}V_0/2,&n=1,\\0,&n\ne1,\end{cases}
$$

by [sine](../../../../../sine.md) [orthogonality](../../../../../orthogonal-vectors.md). For the [cosine](../../../../../cosine.md) coefficients, the product-to-sum identity gives, when $n\ne1$,

$$
\int_0^\pi\sin s\cos ns\,ds
=\frac12\int_0^\pi[\sin((1+n)s)+\sin((1-n)s)]\,ds
=\frac{1+(-1)^n}{1-n^2}.
$$

The case $n=1$ is zero directly. Hence

$$
\boxed{a_{2m}=-\frac{2V_0}{\pi(4m^2-1)},\quad a_{2m-1}=0,\quad
b_1=\frac{V_0}{2},\quad b_n=0\ (n\ne1)}.
$$

The first five nonzero terms, counting the constant as the zero-frequency term, are

$$
\boxed{V_1(t)=\frac{V_0}{\pi}+\frac{V_0}{2}\sin\omega t
-\frac{2V_0}{3\pi}\cos2\omega t
-\frac{2V_0}{15\pi}\cos4\omega t
-\frac{2V_0}{35\pi}\cos6\omega t+\cdots}.
$$

The general coefficient formula specifies every remaining term. This is the [Fourier series of a half-wave rectified sinusoid](../../../../../fourier-series-of-a-half-wave-rectified-sinusoid.md); the waveform is continuous at the joins, so the series gives its actual value there.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

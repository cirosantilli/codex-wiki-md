<h1 id="15/solution">Solution</h1>

↑ **Parent:** [15](../15.md)

Use the real [Fourier series](../../../../fourier-series-split.md) convention $f=a_0/2+\sum_{n\geq1}(a_n\cos nx+b_n\sin nx)$. The [function](../../../../function-split.md) is an [even function](../../../../even-function.md), so $b_n=0$. For noninteger real $\mu$,

$$
a_0=\frac2\pi\int_0^\pi\cos(\mu x)\,dx=\frac{2\sin\pi\mu}{\pi\mu}.
$$

For $n\geq1$, the product-to-sum identity gives

$$
\begin{aligned}
a_n&=\frac1\pi\left(\frac{\sin\pi(\mu-n)}{\mu-n}
+\frac{\sin\pi(\mu+n)}{\mu+n}\right)\\
&=\frac{2\mu(-1)^n\sin\pi\mu}{\pi(\mu^2-n^2)}.
\end{aligned}
$$

Thus the [Fourier series of a noninteger-frequency cosine](../../../../fourier-series-of-a-noninteger-frequency-cosine.md) is

$$
\boxed{f(x)=\frac{\sin\pi\mu}{\pi\mu}
+\frac{2\mu\sin\pi\mu}{\pi}\sum_{n=1}^{\infty}
\frac{(-1)^n\cos nx}{\mu^2-n^2}}.
$$

Its [Fourier coefficients](../../../../fourier-coefficient.md) are $O(n^{-2})$, giving [absolute convergence](../../../../absolute-convergence.md) and [uniform convergence](../../../../uniform-convergence.md). The periodic [function](../../../../function-split.md) is continuous at its joins because the two endpoint cosine values coincide, so the [Dirichlet-Jordan convergence theorem](../../../../dirichlet-jordan-convergence-theorem.md) gives this value at every point.

Putting $\mu=1/3$ gives

$$
\boxed{f(x)=\frac{3\sqrt3}{2\pi}-\frac{3\sqrt3}{\pi}
\sum_{n=1}^{\infty}\frac{(-1)^n\cos nx}{9n^2-1}}.
$$

Evaluate at $x=0$, where $f(0)=1$, and multiply by $\pi/\sqrt3$:

$$
\frac\pi{\sqrt3}=\frac32-3\sum_{n=1}^{\infty}\frac{(-1)^n}{9n^2-1}
=\frac32-\sum_{n=1}^{\infty}\frac{(-1)^n}{3n^2-1/3}.
$$

Comparing with the required form gives $\boxed{A=3,\qquad B=3}$.

## ↑ Ancestors (12)

1. [15](../15.md)
2. [Paper 2](../../paper-2-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

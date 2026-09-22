<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

The function is even, so its [Fourier series](../../../../../fourier-series-split.md) has $b_n=0$. In the convention $f\sim a_0/2+\sum_{n\geq1}(a_n\cos nx+b_n\sin nx)$,

$$
a_0=\frac2\pi\int_0^\pi x^2\,dx=\frac{2\pi^2}{3}.
$$

Twice applying [integration by parts](../../../../../integration-by-parts.md) gives, for $n\geq1$,

$$
\begin{aligned}
\int_0^\pi x^2\cos(nx)\,dx
&=-\frac2n\int_0^\pi x\sin(nx)\,dx\\
&=\frac{2\pi(-1)^n}{n^2},\qquad a_n=\frac{4(-1)^n}{n^2}.
\end{aligned}
$$

Therefore **the periodic Fourier representation is**

$$
\boxed{x^2=\frac{\pi^2}{3}+4\sum_{n=1}^\infty\frac{(-1)^n\cos(nx)}{n^2},\qquad -\pi\leq x\leq\pi,}
$$

with periodic continuation. The periodic extension is continuous, including the identified endpoints, and piecewise smooth, so the [Fourier series](../../../../../fourier-series-split.md) converges to it. The coefficients also give [absolute convergence](../../../../../absolute-convergence.md) and [uniform convergence](../../../../../uniform-convergence.md) by comparison with $\sum n^{-2}$.

At $x=\pi$, the cosine cancels the alternating coefficient sign; at $x=0$, it is identically one. These evaluations yield

$$
\boxed{\sum_{n=1}^\infty\frac1{n^2}=\frac{\pi^2}{6},\qquad \sum_{n=1}^\infty\frac{(-1)^{n+1}}{n^2}=\frac{\pi^2}{12}.}
$$

The first identity solves the [Basel problem](../../../../../basel-problem.md).

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

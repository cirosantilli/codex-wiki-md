<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [separation of variables](../../../../../separation-of-variables.md), let $\Phi=S(\sigma)T(\tau)$. The [Laplace equation](../../../../../laplace-equation.md) gives

$$
-\frac{S''}{S}=\frac{T''}{T}=\lambda.
$$

A nonzero $2\pi$-periodic angular solution requires $\lambda=n^2$, $n=0,1,\ldots$. For $n\geq1$, $S$ is a linear combination of $\cos(n\sigma)$ and $\sin(n\sigma)$, while $T''-n^2T=0$ gives hyperbolic sine and cosine. For $n=0$, periodicity makes $S$ constant, and $T=A_0+B_0\tau$. Negative separation constants would give nonperiodic real exponentials in $\sigma$.

Superposition yields

$$
\boxed{\begin{aligned}
\Phi(\sigma,\tau)={}&A_0+B_0\tau\\
&+\sum_{n=1}^\infty\Big\{[A_n\cosh(n\tau)+B_n\sinh(n\tau)]\cos(n\sigma)\\
&\hspace{40mm}+[C_n\cosh(n\tau)+D_n\sinh(n\tau)]\sin(n\sigma)\Big\}.
\end{aligned}}
$$

Completeness follows by expanding a [harmonic function](../../../../../harmonic-function.md) in a [Fourier series](../../../../../fourier-series-split.md) in the periodic coordinate: its [Fourier coefficients](../../../../../fourier-coefficient.md) must satisfy exactly these radial equations. As usual, the coefficients are restricted by the convergence required of the series on compact subregions. The [bipolar coordinates](../../../../../bipolar-coordinates.md) domain imposes no boundary condition at $\tau=0$ or $\tau=\infty$, so both hyperbolic branches remain available.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

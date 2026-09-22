<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [separation of variables](../../../../../separation-of-variables.md) with $\Phi=M(\mu)N(\nu)$. A nonzero product gives

$$
\frac{M''}{M}=-\frac{N''}{N}=\lambda,\qquad M''-\lambda M=0,\qquad N''+\lambda N=0.
$$

The angular factor must be a [periodic function](../../../../../periodic-function.md) of [period](../../../../../period-of-a-function.md) $2\pi$. If $\lambda<0$, its exponential solutions cannot be periodic unless they vanish. If $\lambda=0$, $N=c+d\nu$ forces $d=0$, while $M=A_0+B_0\mu$. If $\lambda>0$, periodicity requires $\sqrt\lambda=n\in\mathbb N$, giving angular factors $\cos(n\nu),\sin(n\nu)$ and radial factors $\cosh(n\mu),\sinh(n\mu)$.

Superposing these separated [harmonic functions](../../../../../harmonic-function.md) yields

$$
\boxed{\begin{aligned}
\Phi(\mu,\nu)={}&A_0+B_0\mu\\
&+\sum_{n=1}^\infty\Big\{[A_n\cosh(n\mu)+B_n\sinh(n\mu)]\cos(n\nu)\\
&\hspace{45mm}+[C_n\cosh(n\mu)+D_n\sinh(n\mu)]\sin(n\nu)\Big\}.
\end{aligned}}
$$

To see completeness, expand an arbitrary smooth [harmonic function](../../../../../harmonic-function.md) in a [Fourier series](../../../../../fourier-series-split.md) in $\nu$ on each ellipse. Substitution into the equation forces every [Fourier coefficient](../../../../../fourier-coefficient.md) to obey the corresponding radial equation above. The series is interpreted with the convergence needed for a [harmonic function](../../../../../harmonic-function.md), for example locally on compact subannuli. No boundedness condition at infinity or extension across $\mu=0$ has been imposed, so there is no reason to discard either radial branch in these [elliptic coordinates](../../../../../elliptic-coordinates.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

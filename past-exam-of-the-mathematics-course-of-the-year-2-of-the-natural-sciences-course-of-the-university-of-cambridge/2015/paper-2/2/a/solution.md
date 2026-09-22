<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\Phi(r,\theta)=R(r)\Theta(\theta)$ for [separation of variables](../../../../../separation-of-variables.md). Multiplication by $r^2/(R\Theta)$ gives

$$
\frac{r^2R''+rR'}R=-\frac{\Theta''}{\Theta}=\lambda.
$$

Single-valuedness requires a $2\pi$-periodic angular function. The nonzero possibilities are $\lambda=n^2$ for integers $n\geq0$. For $n\geq1$, $\Theta$ is a combination of $\cos n\theta$ and $\sin n\theta$, while the radial [Euler-Cauchy equation](../../../../../euler-cauchy-equation.md) has solutions $r^n,r^{-n}$. At $n=0$, periodicity excludes an angular term proportional to $\theta$, and $(rR')'=0$ gives $R=A_0+B_0\ln r$.

Superposing the separated [harmonic functions](../../../../../harmonic-function.md) yields

$$
\boxed{\begin{aligned}
\Phi(r,\theta)={}&A_0+B_0\ln r\\
&+\sum_{n=1}^\infty\big[(A_nr^n+B_nr^{-n})\cos n\theta+(C_nr^n+D_nr^{-n})\sin n\theta\big].
\end{aligned}}
$$

To obtain the general solution, expand any sufficiently regular harmonic function in a [Fourier series](../../../../../fourier-series-split.md) on circles; each [Fourier coefficient](../../../../../fourier-coefficient.md) satisfies the corresponding radial equation. The coefficients must give the required convergence on compact annuli. Because no condition at zero or infinity is imposed in this part, neither radial branch is discarded.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="14a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [separation of variables](../../../../../../separation-of-variables.md) to the [Laplace equation in polar coordinates](../../../../../../laplace-equation-in-polar-coordinates.md) by writing $\phi(r,\theta)=R(r)\Theta(\theta)$. Division by $R\Theta$ gives

$$
\frac{r(rR')'}R=-\frac{\Theta''}{\Theta}=n^2.
$$

The requirement that $\Theta$ be a real $2\pi$-[periodic function](../../../../../../periodic-function.md) restricts the separation constants to $n^2$, with angular factors $\cos(n\theta)$ and $\sin(n\theta)$. For $n\geq1$, the radial [ordinary differential equation](../../../../../../ordinary-differential-equation.md) is an Euler equation with solutions $r^n$ and $r^{-n}$. For the zero mode, $\Theta$ is constant and

$$
(rR')'=0,
$$

so $R=a_0+c_0\log r$. By [linearity](../../../../../../linearity.md), superposition gives

$$
\boxed{
\begin{aligned}
\phi(r,\theta)
={}&a_0+c_0\log r\\
&+\sum_{n=1}^{\infty}(a_nr^n+c_nr^{-n})\cos(n\theta)\\
&+\sum_{n=1}^{\infty}(b_nr^n+d_nr^{-n})\sin(n\theta).
\end{aligned}
}
$$

This is the separated expansion of a [harmonic function](../../../../../../harmonic-function.md) in a circular region.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

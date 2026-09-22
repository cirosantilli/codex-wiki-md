<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $m=4,n=2$, the equation is the one-dimensional [porous medium equation](../../../../../../../porous-medium-equation.md) $S_\tau=(S^3)_{xx}$. Use a [similarity solution](../../../../../../../similarity-solution.md) $S=\tau^{-1/4}f(\xi)$ and $\xi=x\tau^{-1/4}$. Then

$$
-\frac14(f+\xi f')=(f^3)''.
$$

The no-mass-flux condition at $x=0$ sets the integration constant to zero:

$$
(f^3)'=-\frac14\xi f.
$$

With $f(0)=1$,

$$
\boxed{f(\xi)=\left(1-\frac{\xi^2}{12}\right)_+^{1/2}}.
$$

Consequently

$$
\boxed{\Sigma(r,t)=\Sigma_0\left(\frac r{r_0}\right)^{-3/2}\tau^{-1/4}
\left[1-\frac{r/r_0}{12\tau^{1/2}}\right]_+^{1/2}}.
$$

Its edge is $R=12r_0\tau^{1/2}\propto t^{1/2}$. Moreover,

$$
M=4\pi\Sigma_0r_0^2\int_0^\infty S\,dx
=4\pi\Sigma_0r_0^2\int_0^{\sqrt{12}}f(\xi)d\xi
$$

is time-independent. This agrees with part (b), since $2-m+2n=2$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

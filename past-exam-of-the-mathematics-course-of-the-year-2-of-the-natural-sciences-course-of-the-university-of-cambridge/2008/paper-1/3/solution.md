<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $L=d^2/dx^2+x^{-1}d/dx-x^{-2}$. A [Green's function](../../../../green-s-function-split.md) $G(x,\xi)$ satisfies $L_xG=\delta(x-\xi)$ and the chosen homogeneous [boundary conditions](../../../../boundary-condition.md) in $x$. Away from $x=\xi$, it is a linear combination of $x$ and $x^{-1}$. It must be continuous there and obey the unit derivative jump $G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1$, because the leading differential coefficient is one. Then

$$
y(x)=\int_0^\infty G(x,\xi)f(\xi)\,d\xi
$$

solves $Ly=f$ whenever the integral and boundary limits are valid. The [Wronskian](../../../../wronskian.md) of $x,x^{-1}$ is $-2/x$. The [Green kernels for a radial dipole Euler equation](../../../../green-kernels-for-a-radial-dipole-euler-equation.md) implement the two different choices of boundary conditions below.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

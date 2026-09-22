<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The cooled endpoints impose [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) $\theta(0,t)=\theta(L,t)=0$. The spatial modes are $\sin(n\pi x/L)$. Integrating the initial profile on its two straight segments gives

$$
b_n=\frac2L\left[\int_0^{L/2}x\sin\frac{n\pi x}{L}dx+\int_{L/2}^L(L-x)\sin\frac{n\pi x}{L}dx\right]=\frac{4L}{n^2\pi^2}\sin\frac{n\pi}{2}.
$$

The [heat flow from a triangular initial temperature](../../../../../heat-flow-from-a-triangular-initial-temperature.md) with height $L/2$ is therefore

$$
\boxed{\theta_D(x,t)=\frac{4L}{\pi^2}\sum_{n=1}^\infty\frac{\sin(n\pi/2)}{n^2}\sin\frac{n\pi x}{L}\,e^{-\nu(n\pi/L)^2t}.}
$$

Every nonzero mode decays, so $\theta_D\to0$ as $t\to\infty$. There is no nonzero constant mode compatible with these endpoint temperatures.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

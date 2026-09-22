<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [fundamental solution of the Laplace equation](../../../../../fundamental-solution-of-the-laplace-equation.md) satisfies $\Delta_{\mathbf r}G_0=\delta(\mathbf r-\mathbf r')$ in the sense of [distributions](../../../../../distribution-mathematical-analysis.md), without a boundary condition. Choose it rotationally symmetric about the source. Away from the source, with $s=|\mathbf r-\mathbf r'|$, the radial [Laplace equation](../../../../../laplace-equation.md) is $(sG_0')'=0$, giving $G_0=A\log s+B$.

Integrating over a small disc around the source and using the [divergence theorem](../../../../../divergence-theorem.md) fixes the normalization:

$$
1=\int_{s<\varepsilon}\Delta G_0\,dS
=\int_{s=\varepsilon}\frac{\partial G_0}{\partial s}\,dC
=\frac A\varepsilon\,2\pi\varepsilon=2\pi A.
$$

Therefore

$$
\boxed{G_0(\mathbf r;\mathbf r')=\frac1{2\pi}\log|\mathbf r-\mathbf r'|+B.}
$$

The additive constant is arbitrary; adding other entire [harmonic functions](../../../../../harmonic-function.md) is also possible if rotational symmetry is not imposed. The positive sign here follows from the convention $\Delta G_0=+\delta$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

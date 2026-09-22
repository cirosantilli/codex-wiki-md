<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The two-dimensional [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) is

$$
\boxed{
\partial_t p
=-a_1\partial_xp-\partial_y(a_2p)
+\partial_{xx}p+\frac12\partial_{yy}(\sigma^2p)
=-\nabla\mathbin\cdot\mathbf J,
}
$$

with [Fokker-Planck probability current](../../../../../../fokker-planck-probability-current.md)

$$
\boxed{
\mathbf J=
\left(
a_1p-\partial_xp,\,
a_2p-\frac12\partial_y(\sigma^2p)
\right).
}
$$

The point initial condition is

$$
p(x,y,0)=\delta(x)\delta(y),
$$

where $\delta$ is the [Dirac delta function](../../../../../../dirac-delta-function.md). The [reflecting boundary condition for a diffusion](../../../../../../reflecting-boundary-condition-for-a-diffusion.md) is

$$
\boxed{\mathbf J\mathbin\cdot\mathbf n=0
\quad\hbox{on }\partial\Omega,}
$$

with $\mathbf n$ the outward unit normal. This zero-flux condition conserves the integral of the [probability density function](../../../../../../probability-density-function.md) over the square.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

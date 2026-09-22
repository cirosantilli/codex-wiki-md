<h1 id="16a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the parallel flow $\mathbf u=(u(y,t),0)$ with no pressure gradient, the [Navier-Stokes equations](../../../../../../navier-stokes-equation.md) reduce to the [diffusion equation](../../../../../../diffusion-equation-split.md)

$$
\partial_tu=\nu\,\partial_y^2u.
$$

Substitution of

$$
u=\operatorname{Re}\!\left[U_0f(y)e^{i\omega t}\right]
$$

gives

$$
\nu f''=i\omega f.
$$

The boundary velocities require $f(L_0)=1$ and $f(-L_0)=-1$. The problem is antisymmetric under $y\mapsto-y$, so $f$ is odd. With

$$
k=\sqrt{\frac{i\omega}{\nu}}
=(1+i)\sqrt{\frac{\omega}{2\nu}}
=\frac{(1+i)\Delta}{L_0},
$$

the unique odd solution is

$$
\boxed{
f(y)=\frac{\sinh[(1+i)\Delta\widehat y]}
{\sinh[(1+i)\Delta]},
\qquad
\widehat y=\frac y{L_0},
\qquad
\Delta=\left(\frac{\omega L_0^2}{2\nu}\right)^{1/2}
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16A](../../16a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

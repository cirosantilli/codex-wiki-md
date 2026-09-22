<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At leading order, $X_1=Vt$, $dX_1/dt=V$, $Y_1=0$, and the much smaller motion of sphere 2 may be neglected when evaluating the separation:

$$
\mathbf R\simeq(-X_1,Y_0,0),
\qquad
R=(X_1^2+Y_0^2)^{1/2}.
$$

The $y$ component of the leading $a/R$ term in the mobility from part b is

$$
\frac{dY_2}{dt}
=\frac{3aV}{4R}\frac{R_xR_y}{R^2}
=-\frac{3aV}{4}
\frac{X_1Y_0}{(X_1^2+Y_0^2)^{3/2}}.
$$

Thus

$$
\boxed{
\frac{dY_2/dt}{dX_1/dt}
=-\frac{3a}{4}
\frac{X_1Y_0}{(X_1^2+Y_0^2)^{3/2}}}.
$$

Integrating from the initial position $X_1=0$ to infinity gives the [hydrodynamic displacement of a force-free sphere](../../../../../../hydrodynamic-displacement-of-a-force-free-sphere.md)

$$
\lim_{t\to\infty}[Y_2(t)-Y_0]
=-\frac{3a}{4}
\int_0^\infty
\frac{XY_0}{(X^2+Y_0^2)^{3/2}}\,dX
=\boxed{-\frac{3a}{4}}.
$$

The leading horizontal velocity is

$$
\frac{dX_2}{dt}
=\frac{3aV}{4R}
\left(1+\frac{X_1^2}{R^2}\right)
\sim\frac{3aV}{2X_1}.
$$

Consequently $X_2\sim(3a/2)\log(X_1/Y_0)$ and

$$
\boxed{X_2(t)\longrightarrow+\infty}
$$

logarithmically. The sphere is carried arbitrarily far downstream even though its transverse displacement approaches a finite limit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

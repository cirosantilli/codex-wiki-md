<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

Write $h=r^2\dot\theta$ for the conserved [specific angular momentum](../../../../../specific-angular-momentum.md). Zero [specific orbital energy](../../../../../specific-orbital-energy.md) in the inverse-square [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md) gives

$$
\frac12\left(\dot r^2+\frac{h^2}{r^2}\right)-\frac{GM}r=0.
$$

Define $r_0=h^2/(2GM)$, the [periapsis](../../../../../periapsis.md) radius for a nonradial [parabolic trajectory](../../../../../parabolic-trajectory.md). Then

$$
\dot r^2=\frac{2GM(r-r_0)}{r^2}.
$$

On the outgoing branch, integrate from the [periapsis](../../../../../periapsis.md) time $t_0$ and put $s=\sqrt{r-r_0}$:

$$
\begin{aligned}
t-t_0
&=\frac1{\sqrt{2GM}}\int_{r_0}^r\frac{r'\,dr'}{\sqrt{r'-r_0}}\\
&=\frac2{\sqrt{2GM}}\left(\frac{s^3}3+r_0s\right)
=\frac{\sqrt2}{3\sqrt{GM}}(r+2r_0)\sqrt{r-r_0}.
\end{aligned}
$$

The incoming branch has the opposite sign. Squaring gives the [radius-time relation for a parabolic Kepler orbit](../../../../../radius-time-relation-for-a-parabolic-kepler-orbit.md), a version of the [Barker equation](../../../../../barker-equation.md):

$$
\boxed{(r-r_0)(r+2r_0)^2=\frac92GM(t-t_0)^2.}
$$

Here $r_0$ and $t_0$ are fixed by [angular momentum](../../../../../angular-momentum.md) and the time origin at [periapsis](../../../../../periapsis.md). The relation applies on both branches, with $r\ge r_0$; it is not necessary to solve for the polar angle.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

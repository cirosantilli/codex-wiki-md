<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume an inviscid homogeneous ocean, no horizontal [pressure gradient](../../../../../../pressure-gradient.md), and no [wind stress](../../../../../../wind-stress.md). Horizontal uniformity then removes advective acceleration, and the parcel equations on a [beta plane](../../../../../../beta-plane.md) are

$$
\dot u-f(y)v=0,
\qquad
\dot v+f(y)u=0,
\qquad
f(y)=f_0+\beta y,
$$

with $u=\dot x$ and $v=\dot y$.

Since $\dot u=f(y)\dot y$, integration from the stated initial data gives

$$
\boxed{
\dot x=u=f_0y+\frac12\beta y^2}.
$$

This is conservation of the parcel's zonal canonical momentum: its zonal speed records the meridionally accumulated [Coriolis acceleration](../../../../../../coriolis-acceleration.md). Multiplying the two momentum equations by $u$ and $v$ and adding gives

$$
\frac d{dt}\frac{u^2+v^2}{2}=0.
$$

Thus [kinetic energy](../../../../../../kinetic-energy.md) and speed are constant:

$$
\boxed{\dot x^2+\dot y^2=V^2}.
$$

Eliminating $\dot x$ gives the required [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\boxed{
\dot y^2=V^2-
\left(f_0y+\frac12\beta y^2\right)^2}.
$$

For $f_0,\beta>0$, the equator is at $y_e=-f_0/\beta$. There

$$
f_0y_e+\frac12\beta y_e^2
=-\frac{f_0^2}{2\beta}.
$$

The parcel must encounter a meridional turning point before reaching the equator if it is to remain strictly in the Northern Hemisphere. The energy relation therefore requires

$$
\boxed{
V<\frac{f_0^2}{2\beta}},
$$

or $\beta V/f_0^2<1/2$. Equality is the limiting trajectory that reaches the equator with zero meridional speed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

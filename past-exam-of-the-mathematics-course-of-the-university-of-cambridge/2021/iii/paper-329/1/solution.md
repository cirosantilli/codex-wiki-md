<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a cross-section normal to the cylinder axes, measure $y$ from the line of contact. The two circular boundaries have the [parabolic approximation](../../../../../parabolic-approximation.md)

$$
h(y)=\frac{y^2}{a}+O\left(\frac{y^4}{a^3}\right)
$$

for their separation. The contact point of the meniscus is at $y=w+o(w)$, so the leading cross-sectional area is

$$
\boxed{A(w)=\int_0^w\frac{y^2}{a}\,dy=\frac{w^3}{3a}}.
$$

The area of the small meniscus cap is $O(w^4/a^2)$ and is lower order. At its upper end the gap has width $h(w)=w^2/a$. A tangent semicircle therefore has radius $w^2/(2a)$ and [curvature](../../../../../curvature.md)

$$
\boxed{\kappa=\frac{2a}{w^2}}.
$$

The [Young–Laplace equation](../../../../../young-laplace-equation.md) makes the liquid pressure, relative to the nearly uniform gas pressure,

$$
p=-\gamma\kappa=-\frac{2\gamma a}{w^2},
\qquad
p_z=\frac{4\gamma a}{w^3}w_z.
$$

At a fixed $y$, [lubrication theory](../../../../../lubrication-theory.md) gives a planar [Poiseuille flow](../../../../../hagen-poiseuille-equation.md) through a gap of width $h(y)$, with axial flux per unit $y$

$$
dQ=-\frac{h(y)^3}{12\mu}p_z\,dy.
$$

Integrating across the cusp,

$$
Q=-\frac{p_z}{12\mu}\int_0^w\frac{y^6}{a^3}\,dy
=-\frac{p_zw^7}{84\mu a^3}
=-\frac{\gamma}{21\mu a^2}w^4w_z.
$$

The [continuity equation](../../../../../continuity-equation.md) $A_t+Q_z=0$ now gives

$$
\boxed{
\frac{\partial w^3}{\partial t}
=\frac{\gamma}{7\mu a}
\frac\partial{\partial z}
\left(w^4\frac{\partial w}{\partial z}\right)}.
$$

Set $q=w^3$. Since $w^4w_z=\frac15(q^{5/3})_z$, this is the [porous medium equation](../../../../../porous-medium-equation.md)

$$
q_t=K(q^{5/3})_{zz},
\qquad
K=\frac{\gamma}{35\mu a}.
$$

Conservation of the fixed volume

$$
V=\int_{\mathbb R}A\,dz
=\frac1{3a}\int_{\mathbb R}q\,dz
$$

and [dimensional analysis](../../../../../dimensional-analysis.md) give the [self-similar solution](../../../../../similarity-solution.md) $q=t^{-3/8}F(z/t^{3/8})$. One integration of the resulting ordinary differential equation yields the compactly supported [Barenblatt solution](../../../../../barenblatt-solution.md)

$$
F(\eta)=\left(C-B\eta^2\right)_+^{3/2},
\qquad
B=\frac{21\mu a}{8\gamma}.
$$

Equivalently,

$$
w(z,t)=t^{-1/8}
\left(C-B\frac{z^2}{t^{3/4}}\right)_+^{1/2}.
$$

Its tip is $z_N=(C/B)^{1/2}t^{3/8}$. Using

$$
\int_{-1}^1(1-s^2)^{3/2}\,ds=\frac{3\pi}{8}
$$

in the volume constraint gives $C^2=8aV\sqrt B/\pi$. Therefore

$$
\boxed{
z_N(t)=\left(\frac{8Va}{\pi}\right)^{1/4}
\left(\frac{8\gamma t}{21\mu a}\right)^{3/8}}.
$$

For vertical cylinders at equilibrium, [hydrostatic pressure](../../../../../hydrostatic-pressure.md) gives $p-p_{\rm atm}=-\rho gz$. Balancing this with the [capillary pressure](../../../../../capillary-pressure.md) $-2\gamma a/w^2$ gives the large-height profile

$$
\boxed{w(z)\sim\left(\frac{2\gamma a}{\rho gz}\right)^{1/2}}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 329](../../paper-329-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

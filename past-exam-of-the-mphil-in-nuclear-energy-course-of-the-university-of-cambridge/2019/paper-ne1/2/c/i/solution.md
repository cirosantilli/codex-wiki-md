<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The fundamental nonnegative mode is $\phi_0J_0(2.405r/R)\cos(\pi z/H)$.** Put the origin at the centre of the [cylinder](../../../../../../cylinder-geometry.md), so $-H/2\leq z\leq H/2$. Neglecting extrapolation imposes zero [neutron flux](../../../../../../neutron-flux.md) at $r=R$ and $z=\pm H/2$. Write

$$
B_m^2=\frac{(\eta-1)\Sigma_a}{D},
\qquad
\phi(r,z)=F(r)Z(z).
$$

For an axisymmetric field, [separation of variables](../../../../../../separation-of-variables.md) in [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) gives

$$
\frac{F''+r^{-1}F'}F+\frac{Z''}Z+B_m^2=0.
$$

Choose the axial separation constant so $Z''+\beta^2Z=0$. Midplane symmetry and the lowest positive axial mode give $Z(z)=\cos(\beta z)$, with

$$
\beta H/2=\pi/2,\qquad \beta=\pi/H.
$$

The radial equation is

$$
F''+\frac1rF'+\alpha^2F=0,
\qquad \alpha^2=B_m^2-\beta^2.
$$

The solution regular on the axis is the zero-order [Bessel function of the first kind](../../../../../../bessel-function-of-the-first-kind.md), $F(r)\propto J_0(\alpha r)$; the independent second-kind solution is singular there. The first radial zero gives $\alpha R=j_{0,1}\simeq2.405$. Higher zeros would introduce sign changes and do not describe the fundamental nonnegative [neutron flux](../../../../../../neutron-flux.md). Normalize by the central value, using $J_0(0)=1$:

$$
\boxed{\phi(r,z)=\phi_0J_0(\alpha r)\cos(\beta z),
\qquad \alpha\simeq\frac{2.405}{R},\quad\beta=\frac{\pi}{H}.}
$$

The printed $2.405$ is a rounded [Bessel function](../../../../../../bessel-function-split.md) zero, rather than an exact root.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Module NE1](../../../../paper-ne1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../../split.md)
7. [MPhil in nuclear energy course of the University of Cambridge](../../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

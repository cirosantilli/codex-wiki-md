<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use time dependence $e^{i\omega t}$ and consider fields independent of $y$, with $\mathbf E=\widehat{\mathbf y}E_y(x,z)$. The source-free [Maxwell's equations](../../../../../../maxwell-equations.md) are $\nabla\times\mathbf E=-i\omega\mu\mathbf H$ and $\nabla\times\mathbf H=i\omega\varepsilon\mathbf E$. The first gives

$$
H_x=\frac{\partial_zE_y}{i\omega\mu},
\qquad H_z=-\frac{\partial_xE_y}{i\omega\mu}.
$$

Substitute these into the $y$ component of the second equation. The [TE wave equation in a stratified magnetodielectric](../../../../../../te-wave-equation-in-a-stratified-magnetodielectric.md) is

$$
\boxed{E_{y,xx}+E_{y,zz}-\frac{\mu'}\mu E_{y,z}+\omega^2\mu\varepsilon E_y=0.}
$$

Because its coefficients depend only on $z$, $\partial_xE_y$ obeys the same equation. Since it is proportional to $\mu H_z$, substitution and division by $\mu$ give

$$
\boxed{H_{z,xx}+H_{z,zz}+\frac{\mu'}\mu H_{z,z}
+\left[\omega^2\mu\varepsilon+(\log\mu)''\right]H_z=0.}
$$

For a conserved transverse wavenumber $k_x$, replace $\partial_x^2$ by $-k_x^2$ to obtain the corresponding ordinary [Helmholtz equations](../../../../../../helmholtz-equation.md).

If “propagating along the $z$ axis” is read as strict normal incidence with no $x$ dependence, then $H_z=0$ identically. The nonzero magnetic component is $H_x$, and its equation is

$$
H_x''-\frac{\varepsilon'}{\varepsilon}H_x'+\omega^2\mu\varepsilon H_x=0.
$$

The $H_z$ equation above applies to the oblique [transverse electric polarization](../../../../../../transverse-electric-polarization.md) used in the next part and also includes the zero normal-incidence solution. This distinguishes the named component from the usual transverse magnetic field.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

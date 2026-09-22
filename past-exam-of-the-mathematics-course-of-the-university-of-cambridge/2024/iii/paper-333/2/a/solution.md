<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a steady, small-[Rossby number](../../../../../../rossby-number.md) surface boundary layer, neglect horizontal viscosity and nonlinear acceleration, take the pressure gradient to be independent of depth, impose no normal flow at the surface, and let the viscous stress vanish at $z=-h$. Subtract the depth-independent [geostrophic balance](../../../../../../geostrophic-balance.md) from horizontal momentum. For the ageostrophic velocity,

$$
-fv_a=\nu u_{zz},
\qquad
fu_a=\nu v_{zz}.
$$

Integrating from $-h$ to $0$ and using

$$
\boldsymbol\tau=\rho\nu(u_z,v_z)|_{z=0}
$$

gives the [Ekman transport](../../../../../../ekman-transport.md)

$$
\boxed{
\mathbf M_E=
\int_{-h}^0(u_a,v_a)\,dz
=\left(\frac{\tau_y}{\rho f},
-\frac{\tau_x}{\rho f}\right)
=\frac{\boldsymbol\tau\times\widehat{\mathbf z}}{\rho f}}.
$$

Depth-integrated [mass conservation](../../../../../../mass-conservation.md), with $w(0)=0$, gives

$$
\nabla_h\mathbin\cdot\mathbf M_E-w(-h)=0.
$$

Hence the vertical velocity entering the ocean interior is the [Ekman pumping](../../../../../../ekman-pumping.md) velocity

$$
\boxed{
w_E\equiv w(-h)
=\widehat{\mathbf z}\mathbin\cdot
\nabla_h\times
\left(\frac{\boldsymbol\tau}{\rho f}\right)}.
$$

For constant $f$ this reduces to

$$
\boxed{w_E=\frac{\tau_{y,x}-\tau_{x,y}}{\rho f}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

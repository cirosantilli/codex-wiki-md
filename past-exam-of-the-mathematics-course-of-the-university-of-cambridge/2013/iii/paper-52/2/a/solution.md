<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $e=\rho u^2/2+p/(\gamma-1)$ be the total gas [energy density](../../../../../../energy-density.md), with $\gamma>1$. The one-dimensional continuity and momentum equations are

$$
\partial_t\rho+\partial_z(\rho u)=0,\qquad
\rho(\partial_tu+u\partial_zu)=-\partial_zp.
$$

Using continuity to put the momentum equation into conservative form gives

$$
\partial_t(\rho u)+\partial_z(\rho u^2+p)=0.
$$

The internal [energy density](../../../../../../energy-density.md) $e_{\rm int}=p/(\gamma-1)$ satisfies

$$
\partial_te_{\rm int}+\partial_z(ue_{\rm int})=-p\partial_zu,
$$

by the adiabatic pressure equation. Multiplying the momentum equation by $u$ and using continuity gives

$$
\partial_t\left(\frac{\rho u^2}{2}\right)+\partial_z\left(\frac{\rho u^3}{2}\right)=-u\partial_zp.
$$

Adding these equations combines the pressure work into $-\partial_z(pu)$. The [conservation law](../../../../../../conservation-law.md) variables and [conservation law fluxes](../../../../../../conservation-law-flux.md) are therefore

$$
\boxed{\mathbf U=\begin{pmatrix}\rho\\\rho u\\\rho u^2/2+p/(\gamma-1)\end{pmatrix},\qquad
\mathbf F=\begin{pmatrix}\rho u\\\rho u^2+p\\u\bigl(\rho u^2/2+\gamma p/(\gamma-1)\bigr)\end{pmatrix}.}
$$

The three rows express conservation of mass, momentum and total energy. Their integral [conservation laws](../../../../../../conservation-law.md) remain meaningful across a [shock wave](../../../../../../shock-wave.md), where the differential pressure and velocity equations cannot be applied pointwise.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

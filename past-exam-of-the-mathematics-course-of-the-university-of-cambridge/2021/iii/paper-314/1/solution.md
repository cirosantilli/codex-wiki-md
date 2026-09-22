<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a static spherical star, [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) and the [Poisson equation](../../../../../poisson-equation.md) give

$$
\boxed{\frac{dp}{dr}=-\rho g,
\qquad
g=\frac{d\Phi}{dr}=\frac{Gm(r)}{r^2},
\qquad
\frac{dm}{dr}=4\pi r^2\rho},
$$

or equivalently $r^{-2}d(r^2g)/dr=4\pi G\rho$.

Let $\boldsymbol\xi$ be the fluid [displacement field](../../../../../displacement-field-mechanics.md), so the velocity perturbation is $\delta\mathbf u=\partial_t\boldsymbol\xi$. Linearizing the ideal-fluid momentum equation about the static state and cancelling the background hydrostatic terms gives

$$
\boxed{\rho\frac{\partial^2\boldsymbol\xi}{\partial t^2}
=-\rho\nabla\delta\Phi-\delta\rho\nabla\Phi-\nabla\delta p}.
$$

Conservation of mass says that the Lagrangian density perturbation is $\Delta_L\rho=-\rho\nabla\cdot\boldsymbol\xi$. The relation between [Eulerian and Lagrangian fluid perturbations](../../../../../eulerian-and-lagrangian-fluid-perturbations.md) and adiabatic compression gives, with $\Delta=\nabla\cdot\boldsymbol\xi$,

$$
\boxed{\delta\rho=-\rho\Delta-\boldsymbol\xi\cdot\nabla\rho,
\qquad
\delta p=-\gamma p\Delta-\boldsymbol\xi\cdot\nabla p},
$$

while linearized self-gravity gives $\boxed{\nabla^2\delta\Phi=4\pi G\delta\rho}$.

For the stated [spherical harmonic](../../../../../spherical-harmonic.md) displacement, the radial divergence is $r^{-2}d(r^2\widetilde\xi_r)/dr$, while $\nabla\widetilde\xi_h$ is radial and orthogonal to the angular gradient of $Y_l^m$. Hence

$$
\boxed{\widetilde\Delta
=\frac1{r^2}\frac d{dr}(r^2\widetilde\xi_r)
-k_h^2\widetilde\xi_h,
\qquad
k_h^2=\frac{l(l+1)}{r^2}}.
$$

Equating the radial and horizontal coefficients of $Y_l^m$ and $\nabla Y_l^m$, and applying the separated [Laplacian in spherical coordinates](../../../../../laplacian-in-spherical-coordinates.md) to $\widetilde{\delta\Phi}(r)Y_l^m$, gives

$$
\boxed{-\rho\omega^2\widetilde\xi_r
=-\rho\frac{d\widetilde{\delta\Phi}}{dr}
-g\widetilde{\delta\rho}
-\frac{d\widetilde{\delta p}}{dr}},
$$



$$
\boxed{-\rho\omega^2\widetilde\xi_h
=-\rho\widetilde{\delta\Phi}-\widetilde{\delta p}},
$$



$$
\boxed{\widetilde{\delta\rho}
=-\rho\widetilde\Delta-\widetilde\xi_r\frac{d\rho}{dr},
\qquad
\widetilde{\delta p}
=-\gamma p\widetilde\Delta-\widetilde\xi_r\frac{dp}{dr}},
$$



$$
\boxed{\frac1{r^2}\frac d{dr}
\left(r^2\frac{d\widetilde{\delta\Phi}}{dr}\right)
-k_h^2\widetilde{\delta\Phi}=4\pi G\widetilde{\delta\rho}}.
$$

Define the [stellar buoyancy frequency](../../../../../stellar-buoyancy-frequency.md) by

$$
\boxed{N^2=g\left(
\frac1{\gamma p}\frac{dp}{dr}
-\frac1\rho\frac{d\rho}{dr}\right)}.
$$

Eliminating $\widetilde\Delta$ between the density and pressure perturbations gives

$$
\widetilde{\delta\rho}
=\frac{\rho}{\gamma p}\widetilde{\delta p}
+\frac{\rho N^2}{g}\widetilde\xi_r.
$$

Substitution in the radial equation, followed by use of $dp/dr=-\rho g$, yields

$$
\boxed{(\omega^2-N^2)\widetilde\xi_r
=\frac d{dr}\left(
\widetilde{\delta\Phi}+\frac{\widetilde{\delta p}}\rho\right)
-\frac{N^2\widetilde{\delta p}}{g\rho}}.
$$

Regular spherical profiles near the center have $\rho=\rho_c+O(r^2)$ and $p=p_c+O(r^2)$, while $m(r)=4\pi\rho_cr^3/3+O(r^5)$ and hence $g=O(r)$. Both logarithmic gradients in the definition of $N^2$ are $O(r)$, so $N^2=Ar^2+O(r^4)$. A Sun-like radiative central stratification is stable, making $A>0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 314](../../paper-314-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

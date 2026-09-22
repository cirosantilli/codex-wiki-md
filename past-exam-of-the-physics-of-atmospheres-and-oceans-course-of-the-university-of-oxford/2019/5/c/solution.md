<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a hydrostatic [Boussinesq approximation](../../../../boussinesq-approximation.md), introduce reduced pressure $\pi=p'/\rho_0$ and [buoyancy](../../../../buoyancy.md) $b=-g\rho'/\rho_0$. The [geostrophic balance](../../../../geostrophic-balance.md) and perturbation [hydrostatic balance](../../../../hydrostatic-balance.md) equations are

$$
f u_g=-\pi_y,\qquad f v_g=\pi_x,\qquad\pi_z=b.
$$

Commuting the mixed derivatives gives the height-coordinate [thermal wind](../../../../thermal-wind.md) relations

$$
\boxed{f\frac{\partial u_g}{\partial z}=-\frac{\partial b}{\partial y},\qquad
f\frac{\partial v_g}{\partial z}=\frac{\partial b}{\partial x}.}
$$

Equivalently $u_{g,z}=g\rho'_y/(f\rho_0)$ and $v_{g,z}=-g\rho'_x/(f\rho_0)$. In an atmosphere the corresponding ideal-gas form is conveniently derived from geopotential $\Phi$ on pressure surfaces: $fu_g=-\Phi_y|_p$, $fv_g=\Phi_x|_p$, and $\Phi_{\ln p}=-R_aT$. Hence

$$
f u_{g,\ln p}=R_aT_y|_p,\qquad f v_{g,\ln p}=-R_aT_x|_p.
$$

Since $d\ln p/dz=-g/(R_aT)$, this gives the vertical shear at a fixed horizontal location,

$$
\boxed{u_{g,z}=-\frac{g}{fT}T_y\big|_p,\qquad v_{g,z}=\frac{g}{fT}T_x\big|_p.}
$$

The horizontal temperature derivatives here are on isobars; replacing them by fixed-height derivatives is a small-slope approximation. This qualification avoids mixing compressible and Boussinesq density gradients.

For an illustrative poleward temperature drop $40\,\mathrm K$ across $3000\,\mathrm{km}$, mean $T\sim250\,\mathrm K$, $f\sim10^{-4}\,\mathrm{s^{-1}}$ and depth $10\,\mathrm{km}$,

$$
\boxed{\Delta u_g\sim\frac{gH\Delta T}{fT L}\simeq52\,\mathrm{m\,s^{-1}}.}
$$

Adding a modest surface wind gives an upper-level westerly jet of order $50$–$60\,\mathrm{m\,s^{-1}}$. The [thermal wind](../../../../thermal-wind.md) fixes vertical shear, not the absolute wind without a boundary or reference value.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

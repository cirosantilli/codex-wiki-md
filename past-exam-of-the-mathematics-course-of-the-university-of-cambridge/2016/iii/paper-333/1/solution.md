<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use an upward vertical coordinate $z$, constant [mass density](../../../../../density.md) $\rho$, and a positive [Coriolis parameter](../../../../../coriolis-parameter.md) $f$; the square-root formulas below assume the Northern Hemisphere. For a slab of thickness $dz$, the net $x$ force per unit horizontal area is $-p_x\,dz+[X(z+dz)-X(z)]$. Dividing by its mass $\rho\,dz$ and including the [Coriolis acceleration](../../../../../coriolis-acceleration.md) gives

$$
u_t-fv=-\frac{p_x}{\rho}+\frac{X_z}{\rho},\qquad v_t+fu=-\frac{p_y}{\rho}+\frac{Y_z}{\rho}.
$$

Here $X,Y$ are the vertical [shear stress](../../../../../shear-stress.md) components of the [viscous stress tensor](../../../../../viscous-stress-tensor.md), so their boundary values require a signed traction convention. Linearization removes advective acceleration. Decompose the horizontal velocity into an exterior pressure response and an [Ekman layer](../../../../../ekman-layer.md) correction. On an [f-plane](../../../../../f-plane.md) these satisfy

$$
u_t^P-fv^P=-p_x/\rho,\qquad v_t^P+fu^P=-p_y/\rho,
$$

and

$$
u_t^E-fv^E=X_z/\rho,\qquad v_t^E+fu^E=Y_z/\rho.
$$

The exterior pressure response is in [geostrophic balance](../../../../../geostrophic-balance.md) when steady. For a [surface Ekman layer](../../../../../surface-ekman-layer.md) with negligible stress at its base, its [Ekman transport](../../../../../ekman-transport.md) is

$$
M_x^E=\int u^E\,dz=\frac{Y^s}{\rho f},\qquad M_y^E=\int v^E\,dz=-\frac{X^s}{\rho f}.
$$

Integrating the [continuity equation](../../../../../continuity-equation.md) and imposing zero vertical boundary-layer velocity at the surface gives $w_b^E=\partial_xM_x^E+\partial_yM_y^E$. **Thus the base velocity, positive upward, is**

$$
\boxed{w_b^E=\frac{Y_x^s-X_y^s}{\rho f}.}
$$

The PDF prints the opposite sign. Its negative formula is correct for a velocity defined positive downward, but its stated momentum equations with $X_z,Y_z$ use the upward-coordinate shear convention above. This sign must be accounted for when interpreting the subsequent pumping equation.

For constant [kinematic viscosity](../../../../../kinematic-viscosity.md), write $W_E=u^E+iv^E$ and $\delta=\sqrt{2\nu/f}$. The steady [Ekman layer](../../../../../ekman-layer.md) equation is $\nu W_E''=ifW_E$. Taking the surface at $z=0$ and the ocean below it, the bounded [surface Ekman layer](../../../../../surface-ekman-layer.md) solution is

$$
\boxed{W_E(z)=\frac{X^s+iY^s}{\rho\nu\lambda}\,e^{\lambda z},\qquad \lambda=\frac{1+i}{\delta},\quad z\le0.}
$$

The total velocity is $W_P+W_E$. Prescribed [wind stress](../../../../../wind-stress.md) determines the coefficient of this [Ekman layer](../../../../../ekman-layer.md) correction; it does not determine a relation between the wind and the independent pressure-driven velocity. **An additional boundary condition is necessary for a [laminar Ekman boundary stress](../../../../../laminar-ekman-boundary-stress.md) law in terms of $u^P,v^P$.**

The two printed laminar stress formulas and the positive pressure-Laplacian pumping formula are instead the standard [Bottom Ekman layer](../../../../../bottom-ekman-layer.md) relations. To derive them consistently, put a stationary [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $z=0$, with water at $z>0$. Then

$$
W_E=-W_Pe^{-(1+i)z/\delta},\qquad X_b+iY_b=\rho\nu W_E'(0)=\rho\sqrt{\frac{f\nu}{2}}(1+i)W_P.
$$

Consequently

$$
\boxed{X_b=\rho\sqrt{\frac{f\nu}{2}}(u^P-v^P),\qquad Y_b=\rho\sqrt{\frac{f\nu}{2}}(u^P+v^P).}
$$

These are [shear stress](../../../../../shear-stress.md) values; the actual bottom traction on the fluid has the opposite sign. Integrating this [Bottom Ekman layer](../../../../../bottom-ekman-layer.md) gives $M_x^E=-\delta(u^P+v^P)/2$ and $M_y^E=\delta(u^P-v^P)/2$. Since the exterior [geostrophic flow](../../../../../geostrophic-flow.md) is horizontally nondivergent, the upward velocity above the bottom is $-\nabla_h\cdot\mathbf M_E=\delta\zeta_P/2$. Using $u^P=-p_y/(\rho f)$, $v^P=p_x/(\rho f)$ yields

$$
\boxed{w_b=\frac{1}{\rho f}\sqrt{\frac{\nu}{2f}}\,\nabla_h^2p.}
$$

This recovers the requested magnitude and pressure dependence with a consistent bottom interpretation. The surface version would require its own specified boundary velocity and corresponding signs.

For [Ekman spin-down in a shallow-water layer](../../../../../ekman-spin-down-in-a-shallow-water-layer.md), let $\alpha=\sqrt{f\nu/2}$, $c^2=gH$, and $R_D=c/f$. Upward bottom pumping enters the exterior [linearized shallow water equations](../../../../../linearized-shallow-water-equations.md) through $\eta_t+H\nabla_h\cdot\mathbf u=w_b$. Taking the curl of their momentum equations gives $\zeta_t+f\nabla_h\cdot\mathbf u=0$, hence

$$
\left(\zeta-\frac{f\eta}{H}\right)_t=-\frac{f}{H}w_b.
$$

Slow [geostrophic balance](../../../../../geostrophic-balance.md) gives $\zeta=(g/f)\nabla_h^2\eta$ and $w_b=(g\alpha/f^2)\nabla_h^2\eta$. Therefore the intended damping equation is

$$
\boxed{(\nabla_h^2\eta-R_D^{-2}\eta)_t=-\frac{\alpha}{H}\nabla_h^2\eta.}
$$

**The slow-adjustment assumption is $f\tau\gg1$, not the printed $f\tau\ll1$.** The printed negative pumping term in continuity can alternatively describe downward extraction at the upper boundary, but it cannot be combined unchanged with the upward bottom pumping just derived. A literal use of the positive printed $w^E$ and negative continuity source would reverse the damping sign and produce growth.

For a [Fourier mode](../../../../../fourier-mode.md) $\eta=\widehat\eta(t)e^{i\mathbf k\cdot\mathbf x}$ with $|\mathbf k|=\kappa>0$, substitution gives

$$
\widehat\eta_t=-\frac{\alpha}{H}\frac{\kappa^2}{\kappa^2+R_D^{-2}}\widehat\eta,\qquad \boxed{\tau=\frac{H}{\alpha}\left(1+\frac{1}{\kappa^2R_D^2}\right).}
$$

For scales small compared with the [Rossby deformation radius](../../../../../rossby-deformation-radius.md), $\kappa R_D\gg1$ and $\tau\simeq H/\alpha$, independent of [wavenumber](../../../../../wavenumber.md). For scales large compared with the [Rossby deformation radius](../../../../../rossby-deformation-radius.md), the equation becomes $\eta_t=K^E\nabla_h^2\eta$, where

$$
\boxed{K^E=\frac{\alpha R_D^2}{H}=\frac{g}{f^2}\sqrt{\frac{f\nu}{2}}.}
$$

The zero [wavenumber](../../../../../wavenumber.md) mode does not decay. A thin [Ekman layer](../../../../../ekman-layer.md), $\delta/H\ll1$, makes $fH/\alpha=2H/\delta\gg1$, so the derived decay time satisfies the corrected slow-time assumption.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

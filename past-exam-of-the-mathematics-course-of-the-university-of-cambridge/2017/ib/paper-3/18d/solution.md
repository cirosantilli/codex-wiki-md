<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

For constant-density incompressible inviscid flow with conservative body force, [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) give $\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\nabla(p/\rho+\Phi)$. Using $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$, take the [curl](../../../../../curl.md) to obtain $\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega)$. Since both divergences vanish, the vector identity expands this to

$$
\boxed{\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

Without incompressibility or the constant-density/barotropic hypothesis, extra compression or baroclinic terms are present; the printed equation uses these flow assumptions.

Let $\kappa(t)=\dot h/h$, with $h>0$. Axisymmetric [mass conservation](../../../../../mass-conservation.md) is $r^{-1}\partial_r(ru_r)+\partial_zu_z=0$. If $u_r$ is independent of $z$, then $u_z$ is affine in $z$. The impermeable moving-plate conditions $u_z(r,\pm h,t)=\pm\dot h$ force $u_z=\kappa z$, and integrating the radial equation gives $u_r=-\kappa r/2+C(t)/r$. Regularity at the axis excludes $C(t)/r$. The meridional part of the [axisymmetric inviscid flow between moving parallel plates](../../../../../axisymmetric-inviscid-flow-between-moving-parallel-plates.md) is therefore

$$
\boxed{u_r=-\frac{\dot h}{2h}r,\qquad u_z=\frac{\dot h}{h}z.}
$$

For no swirl, $u_\theta=0$ completes the field. Continuity alone does not determine azimuthal motion; this must be specified separately. More generally, prescribe a smooth regular initial profile $U(r)$ independent of $z$. The azimuthal part of [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) is

$$
\partial_tu_\theta-\frac{\kappa r}{2}\partial_ru_\theta-\frac\kappa2u_\theta=0,
$$

so conservation of $r u_\theta$ along radial particle paths gives $u_\theta(r,t)=\lambda U(\lambda r)$, where $\lambda=\sqrt{h/h_0}$. Together with the meridional components above, this gives a family of complete fields, with a suitable [pressure](../../../../../pressure.md) determined by the radial and vertical equations. The field is therefore not unique without rotational data.

With the stated solid-body rotation, $u_\theta=\Omega(t)r$ and $\boldsymbol\omega=2\Omega\mathbf e_z$. The [vorticity equation](../../../../../vorticity-equation.md) gives $2\dot\Omega=2\Omega\partial_zu_z=2\Omega\kappa$, hence

$$
\boxed{\Omega(t)=\Omega_0\frac{h(t)}{h_0},\qquad
\mathbf u=-\frac{\dot h}{2h}r\,\mathbf e_r+\Omega_0\frac h{h_0}r\,\mathbf e_\theta+\frac{\dot h}{h}z\,\mathbf e_z.}
$$

For a fluid particle, $\dot r=-\kappa r/2$, so $r^2h$ is constant and $r^2\Omega$ is constant. This is [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) about the axis: radial spreading when the plates approach decreases the angular velocity. The meridional and rotating fields satisfy the inviscid equations with an appropriate pressure; no tangential no-slip condition is imposed on inviscid plates.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

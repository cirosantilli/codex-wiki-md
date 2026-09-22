<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In a steady flow the [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives $\nabla\times(\mathbf u\times\mathbf B)=0$. Since both vectors have only [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) components, write $\mathbf u\times\mathbf B=F_\phi\mathbf e_\phi$. Axisymmetry implies

$$
\partial_zF_\phi=0,\qquad \partial_R(RF_\phi)=0,
\qquad F_\phi=\frac{C}{R}.
$$

For a field regular on the axis, $C=0$; equivalently one may impose zero toroidal [electromotive force](../../../../../electromotive-force.md). Under this physical condition, $\mathbf u$ is parallel to $\mathbf B$. Write $\rho\mathbf u=k\mathbf B$. Continuity and $\nabla\cdot\mathbf B=0$ then give $\mathbf B\cdot\nabla k=0$. The [poloidal magnetic flux function](../../../../../poloidal-magnetic-flux-function.md) has $\mathbf B\cdot\nabla\psi=0$, so locally on each connected magnetic surface,

$$
\boxed{\mathbf u=\frac{k(\psi)}{\rho}\mathbf B.}
$$

This [regular-axis alignment of steady poloidal ideal flow](../../../../../regular-axis-alignment-of-steady-poloidal-ideal-flow.md) needs its zero-circulation condition: axisymmetry alone does not imply this alignment on a domain excluding the axis. An explicit counterexample is available in a cylindrical annulus. Take nonzero constants $U,b$, positive $\rho_c,c_s$, and

$$
\mathbf u=U\mathbf e_z,\quad \mathbf B=\frac bR\mathbf e_R,\quad
\rho=\frac{\rho_c}{(1+R^2/a^2)^2},\quad p=c_s^2\rho,\quad
\Phi=2c_s^2\ln(1+R^2/a^2),\quad a^2=\frac{2c_s^2}{\pi G\rho_c}.
$$

Here $\psi=-bz$, $\nabla\cdot\mathbf B=\nabla\times\mathbf B=0$ and $\mathbf u\times\mathbf B=Ub\mathbf e_\phi/R$ has zero [curl](../../../../../curl.md). The flow satisfies continuity, $p'=-\rho\Phi'$, and $\nabla^2\Phi=4\pi G\rho$. Its acceleration and [Lorentz force density](../../../../../lorentz-force-density.md) vanish, so it solves the steady equations while $\mathbf u$ and $\mathbf B$ are perpendicular. The nonzero toroidal circulation and the axial singularity explain why this counterexample is excluded from a regular polar [accretion column](../../../../../accretion-column.md). The remaining derivation uses the regular, aligned branch.

For a narrow [stream tube](../../../../../stream-tube.md), integrating continuity gives constant $A\rho|\mathbf u|$. On a nonzero-flow tube the [magnetohydrodynamic mass loading](../../../../../magnetohydrodynamic-mass-loading.md) $k$ is constant, so $A\rho|\mathbf u|=A|k||\mathbf B|$. Therefore **$A|\mathbf B|$ is constant and $A\propto|\mathbf B|^{-1}$.** This also follows directly from conserved [magnetic flux](../../../../../magnetic-flux.md) through a [flux tube](../../../../../flux-tube.md).

For constant [isothermal sound speed](../../../../../isothermal-sound-speed.md), $\nabla p/\rho=c_s^2\nabla\ln(\rho/\rho_0)$, with arbitrary reference density $\rho_0$. Project momentum along $\mathbf B$. The [Lorentz force density](../../../../../lorentz-force-density.md) has no component in that direction, and alignment implies $\mathbf B\cdot(\mathbf u\cdot\nabla)\mathbf u=\mathbf B\cdot\nabla(|\mathbf u|^2/2)$. Thus the [isothermal magnetic Bernoulli integral](../../../../../isothermal-magnetic-bernoulli-integral.md) is

$$
\boxed{\frac12|\mathbf u|^2+\Phi+c_s^2\ln(\rho/\rho_0)=\epsilon(\psi).}
$$

Changing $\rho_0$ only shifts the [Bernoulli function](../../../../../bernoulli-function.md) by a constant. Since $k$ is constant along the [magnetic field](../../../../../magnetic-field.md),

$$
\mathbf B\cdot\nabla\left(\frac{|\mathbf u|^2}{2}\right)
=|\mathbf u|^2\left[\mathbf B\cdot\nabla\ln|\mathbf B|-\frac{\mathbf B\cdot\nabla\rho}{\rho}\right].
$$

Differentiating the [isothermal magnetic Bernoulli integral](../../../../../isothermal-magnetic-bernoulli-integral.md) therefore gives

$$
\boxed{(c_s^2-|\mathbf u|^2)\mathbf B\cdot\nabla\rho
=-\rho\left[\mathbf B\cdot\nabla\Phi+|\mathbf u|^2\mathbf B\cdot\nabla\ln|\mathbf B|\right].}
$$

In the slender polar [accretion column](../../../../../accretion-column.md), the [dipolar flux-tube area](../../../../../dipolar-flux-tube-area.md) is $A(z)=A_*(z/R_*)^3$. The decreasing axial field is a leading approximation, not an exactly solenoidal field $(0,0,B_z(z))$ throughout a cylinder. Indeed $\nabla\cdot\mathbf B=\partial_zB_z\ne0$ for that literal field. Near the axis a small radial component $B_R\simeq-(R/2)\partial_zB_z=3RB_z/(2z)$ supplies the required radial divergence. Its magnitude is smaller by $R/z$, even though its divergence is leading order. Keeping this expanding [flux tube](../../../../../flux-tube.md) while neglecting transverse forces yields the intended one-dimensional model.

Use the positive inward speed $v=-u_z$; the signed sonic velocity is $u_z=-c_s$. Conservation of mass and the [Bernoulli equation](../../../../../bernoulli-equation.md) give

$$
A\rho v=\dot M,\quad \frac{\rho'}{\rho}=-\frac{v'}v-\frac3z,\quad
vv'+\frac{GM_*}{z^2}+c_s^2\frac{\rho'}\rho=0.
$$

Eliminating $\rho'$ yields the [isothermal dipolar accretion equation](../../../../../isothermal-dipolar-accretion-equation.md),

$$
\left(v-\frac{c_s^2}{v}\right)v'=\frac{3c_s^2}{z}-\frac{GM_*}{z^2}.
$$

A smooth [transonic branch](../../../../../transonic-branch.md) requires both sides to vanish at its [sonic point](../../../../../sonic-point.md), so

$$
\boxed{v_s=c_s,\qquad z_s=\frac{GM_*}{3c_s^2}.}
$$

This is the critical point of the flow equation; a generic subsonic solution need not cross it. A crossing in the exterior column requires $z_s\geq R_*$, and a sonic point strictly outside the star requires $z_s>R_*$. Differentiating the equation at the crossing gives $2(v_s')^2=3c_s^2/z_s^2$. For inward accretion that accelerates toward the star, $v_s'=-\sqrt{3/2}\,c_s/z_s$.

The reservoir boundary condition fixes $\epsilon=c_s^2\ln(\rho_\infty/\rho_0)$. At the [sonic point](../../../../../sonic-point.md), $\Phi_s=-3c_s^2$ and $v_s^2/2=c_s^2/2$, giving

$$
\ln\frac{\rho_s}{\rho_\infty}=3-\frac12=\frac52,
\qquad \boxed{\rho_s=e^{5/2}\rho_\infty.}
$$

Finally use the sonic [mass flux](../../../../../mass-flux.md) through the [dipolar flux-tube area](../../../../../dipolar-flux-tube-area.md):

$$
\boxed{\dot M=\rho_\infty c_sA_*e^{5/2}\left(\frac{GM_*}{3c_s^2R_*}\right)^3.}
$$

This rate belongs to the smooth [transonic branch](../../../../../transonic-branch.md) of the idealized column, with $A_*$ the supplied total loaded area. The reservoir condition alone does not force every steady solution onto this branch. A real narrow dipolar column must match an outer flow where the slender approximation ceases to apply.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

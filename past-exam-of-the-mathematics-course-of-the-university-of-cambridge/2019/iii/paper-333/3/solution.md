<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $D_g=\partial_t+\mathbf u_g\cdot\nabla_h$, $\psi=\widetilde\Phi/f_0$, and $\mathbf u_g=(-\psi_y,\psi_x,0)$. The hydrostatic and thermal equations combine to give

$$
D_g\psi_z=-\frac{N^2}{f_0}w,\qquad \boxed{N^2=\frac{RS(z)}H.}
$$

Taking the vertical [curl](../../../../../curl.md) of the horizontal momentum equations to leading quasi-geostrophic order gives

$$
D_g\nabla_h^2\psi+\beta\psi_x+f_0\nabla_h\cdot\mathbf u_{a,h}=0.
$$

The [log-pressure coordinate](../../../../../log-pressure-coordinate.md) continuity equation gives $\nabla_h\cdot\mathbf u_{a,h}=-e^{z/H}\partial_z(e^{-z/H}w)$. Substitute $w=-f_0D_g\psi_z/N^2$. In commuting the vertical derivative with $D_g$, the extra term is $\mathbf u_{g,z}\cdot\nabla_h\psi_z=(-\psi_{yz},\psi_{xz})\cdot(\psi_{xz},\psi_{yz})=0$. Therefore the [log-pressure quasi-geostrophic potential vorticity](../../../../../log-pressure-quasi-geostrophic-potential-vorticity.md) equation is

$$
\boxed{D_g\left[\psi_{xx}+\psi_{yy}+e^{z/H}\partial_z\left(e^{-z/H}\frac{f_0^2}{N^2}\psi_z\right)\right]+\beta\psi_x=0.}
$$

The required small parameters have distinct roles. The [Rossby number](../../../../../rossby-number.md) $\epsilon_R=U/(|f_0|L)$ makes inertial acceleration small relative to the leading [geostrophic balance](../../../../../geostrophic-balance.md). The parameter $\epsilon_\beta=\beta L/|f_0|$ lets that leading balance use a single $f_0$ while retaining the beta effect in the slower vorticity evolution. Finally, $\psi\sim UL$ and the thermal equation imply $w\sim |f_0|U^2/(N^2D)$. Density-weighted continuity has vertical derivative scale $1/\delta$, where $\delta=\min(D,H)$, so $|\mathbf u_{a,h}|\sim Lw/\delta$. The [vertical-advection consistency criterion for log-pressure quasi-geostrophy](../../../../../vertical-advection-consistency-criterion-for-log-pressure-quasi-geostrophy.md) is thus

$$
\boxed{\frac{|\mathbf u_{a,h}|}{U}\sim\epsilon_a=\frac{f_0^2L^2H}{RSD\min(D,H)}\frac{U}{|f_0|L}\ll1.}
$$

It also controls the omitted vertical-advection ratio $wL/(UD)\sim\epsilon_a\delta/D$. Small Rossby number alone would not ensure small [ageostrophic flow](../../../../../ageostrophic-flow.md) for every choice of stratification and vertical scales.

For constant $N$, linearization about rest gives

$$
\partial_t\left[\nabla_h^2\psi+\frac{f_0^2}{N^2}\left(\psi_{zz}-\frac1H\psi_z\right)\right]+\beta\psi_x=0.
$$

Putting $\psi=\operatorname{Re}[\widehat\psi_c e^{z/(2H)}e^{i(kx+mz-\omega t)}]$ replaces the vertical operator by $-m^2-1/(4H^2)$. Consequently the [Rossby wave in a log-pressure atmosphere](../../../../../rossby-wave-in-a-log-pressure-atmosphere.md) has

$$
\boxed{\omega=-\frac{\beta k}{k^2+(f_0^2/N^2)[m^2+1/(4H^2)]}.}
$$

For the forced half-space, substitution of the specified ansatz gives

$$
\widehat\chi''+m^2\widehat\chi=0,\qquad m^2=-\frac1{4H^2}-\frac{N^2}{f_0^2}\left(k^2+\frac{\beta k}{\omega}\right),\qquad \widehat\chi(0)=\Psi_b.
$$

Assume $\beta>0$ and $k>0$, and define $\omega_*=-\beta k/[k^2+f_0^2/(4N^2H^2)]<0$.

If $\omega>0$ or $\omega<\omega_*$, then $m^2<0$. Boundedness excludes the growing solution and uniquely selects $\boxed{\widehat\chi=\Psi_b e^{-\sqrt{-m^2}\,z}}$. If $\omega=\omega_*$, boundedness excludes the linear-in-$z$ solution, leaving $\widehat\chi=\Psi_b$; this is the zero-vertical-wavenumber threshold.

If $\omega_*<\omega<0$, both oscillatory solutions are bounded. **Boundedness alone does not give a unique propagating solution.** With forcing at the bottom and no incident wave from above, impose an upward [radiation condition](../../../../../radiation-condition.md). Since

$$
\frac{\partial\omega}{\partial m}=\frac{2\beta k(f_0^2/N^2)m}{[k^2+(f_0^2/N^2)(m^2+1/(4H^2))]^2},
$$

positive $m$ has upward [group velocity](../../../../../group-velocity.md). The outgoing solution is $\boxed{\widehat\chi=\Psi_b e^{imz},\quad m=\sqrt{m^2}>0}$. The physical streamfunction includes the prescribed $e^{z/(2H)}$ density-weighting factor; it is the amplitude $\widehat\chi$ that must remain bounded.

Thus the strict range for vertically propagating waves is

$$
\boxed{-\frac{\beta k}{k^2+f_0^2/(4N^2H^2)}<\omega<0.}
$$

At $\omega=0$, the unforced steady interior equation requires $\beta\psi_x=0$, so a nonzero $k$ bottom streamfunction cannot have a time-independent solution of this ideal rest-state problem without additional dynamics.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Balanced variables and PV derivation.** Write the disturbance reduced [pressure](../../../../../pressure.md) as $p'/\rho_0=f_0\psi$. Leading [geostrophic balance](../../../../../geostrophic-balance.md) gives $(u_g,v_g)=(-\psi_y,\psi_x)$, and leading hydrostatic balance gives [buoyancy](../../../../../buoyancy.md) anomaly $\sigma'=p'_z/\rho_0=f_0\psi_z$. The geostrophic [material derivative](../../../../../material-derivative.md) is

$$
\frac{D_g}{Dt}=\partial_t-\psi_y\partial_x+\psi_x\partial_y.
$$

It includes horizontal advection, not an independent prognostic vertical velocity. The appropriate regime has small [Rossby number](../../../../../rossby-number.md), small stratified [Froude number](../../../../../froude-number.md), thin aspect ratio and slow evolution; a common scaling has $[NH/(f_0L)]^2$ of order one and $\beta L/|f_0|\ll1$.

Only the vertical rotation component is retained in the [traditional approximation](../../../../../traditional-approximation-geophysical-fluid-dynamics.md). In the horizontal momentum balance, the horizontal part of the rotation vector multiplies the small vertical velocity; in vertical momentum, its contribution is small compared with leading hydrostatic [pressure](../../../../../pressure.md) and [buoyancy](../../../../../buoyancy.md) in the thin-layer scaling. Away from the equator these corrections are smaller by a factor of order $(H/L)\cot\lambda$. They need not be small in equatorial or strongly nonhydrostatic settings, so the approximation has a definite regime of validity.

Put $A(z)=f_0^2/N^2(z)$. Eliminating $w$ from [buoyancy](../../../../../buoyancy.md) gives

$$
f_0 w_z=-\partial_z[D_g(A\psi_z)]
=-D_g\partial_z(A\psi_z).
$$

The last step needs justification because $D_g$ and $\partial_z$ do not commute on arbitrary fields. Their extra terms here are

$$
u_{g,z}\partial_x(A\psi_z)+v_{g,z}\partial_y(A\psi_z)
=A(-\psi_{yz}\psi_{xz}+\psi_{xz}\psi_{yz})=0.
$$

Substitution into the supplied [vorticity](../../../../../vorticity.md) equation gives

$$
D_g[\nabla_h^2\psi+\partial_z(A\psi_z)]+\beta\psi_x=0.
$$

Since $D_gf=\beta v_g=\beta\psi_x$,

$$
\boxed{\frac{D_gQ}{Dt}=0,\qquad Q=f+\psi_{xx}+\psi_{yy}+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right).}
$$

This is [three-dimensional quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) conservation; the height-dependent coefficient is retained inside the derivative.

At a small steady lower elevation $b(x,y)$, impermeability gives $w=u_gb_x+v_gb_y=D_gb$, evaluated at $z=0$ to leading order. Substitution into [buoyancy](../../../../../buoyancy.md) and division by $N^2$ gives the [topographic buoyancy boundary condition for quasi-geostrophic flow](../../../../../topographic-buoyancy-boundary-condition-for-quasi-geostrophic-flow.md),

$$
\boxed{\frac{D_g}{Dt}\left(\frac{f_0}{N^2}\psi_z+b\right)=0\quad\text{at }z=0.}
$$

**[Rossby waves](../../../../../rossby-wave.md) at rest.** For constant $N$ let $\alpha=f_0^2/N^2$ and $K^2=k^2+\alpha m^2$. Linearization about relative rest gives $\partial_t(\psi_{xx}+\alpha\psi_{zz})+\beta\psi_x=0$. A Fourier wave gives

$$
\boxed{\omega=-\frac{\beta k}{k^2+\alpha m^2}.}
$$

For $\beta>0$, the zonal phase speed $\omega/k=-\beta/K^2$ is westward. At fixed altitude the PV perturbation is $q'=-K^2\psi'$; its total field is the background $f_0+\beta y$ with sinusoidally displaced contours, as sketched below.

<a id="3/image-rossby-wave-pv-contours-and-meridional-flow-producing-westward-phase-propagation"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-80-rossby-pv.png)

**[Figure 1](#3/image-rossby-wave-pv-contours-and-meridional-flow-producing-westward-phase-propagation). Rossby-wave PV contours and meridional flow producing westward phase propagation**.

A northward parcel displacement has $q'=-\beta\xi_y$: it retains the smaller background PV of its origin. The inverted geostrophic velocity associated with a positive PV crest is northward on its eastern flank and southward on its western flank. Advection of the background PV then decreases the anomaly on the eastern flank and increases it on the western flank, shifting the crest westward. This is a PV-restoring mechanism, not a westward mean current.

Differentiating the dispersion relation gives the [group velocity](../../../../../group-velocity.md)

$$
\boxed{c_{gx}=\frac{\beta(k^2-\alpha m^2)}{(k^2+\alpha m^2)^2},\qquad
c_{gz}=\frac{2\beta\alpha km}{(k^2+\alpha m^2)^2},\qquad c_{gy}=0.}
$$

For nonzero $k,m$, the vertical phase speed is $\omega/m=-\beta k/[m(k^2+\alpha m^2)]$, so

$$
c_{gz}\frac{\omega}{m}=-\frac{2\beta^2\alpha k^2}{(k^2+\alpha m^2)^3}<0.
$$

Thus upward energy propagation accompanies downward vertical phase propagation, and conversely. For $m=0$ the vertical group speed is zero and a vertical phase speed is not defined.

**Stationary topographic response.** Assume $f_0\ne0$, $\beta>0$ and nonzero corrugation [wavenumber](../../../../../wavenumber.md) $k$. In a uniform current the laboratory dispersion is $\omega_{\mathrm{lab}}=Uk-\beta k/K^2$. For a stationary [quasi-geostrophic mountain wave](../../../../../quasi-geostrophic-mountain-wave.md), $K^2=\beta/U$, giving

$$
m^2=\frac{N^2}{f_0^2}\left(\frac\beta U-k^2\right).
$$

For $U\ne0$, the linear lower-boundary condition becomes $U\partial_x[(f_0/N^2)\psi'_z+b]=0$. Its forced nonzero-$k$ component therefore has

$$
\psi'_z(0)=-\frac{N^2b_0}{f_0}\sin kx.
$$

If $0<U<\beta/k^2$, the vertical [wavenumber](../../../../../wavenumber.md) is real. Both signs would be bounded aloft, so boundedness alone is insufficient for uniqueness. Impose an upward [radiation condition](../../../../../radiation-condition.md), excluding waves incident from infinity; equivalently switch on the terrain forcing causally with arbitrarily weak absorption aloft. Since $c_{gz}$ has the sign of $km$, choose

$$
m=\operatorname{sgn}(k)\frac N{|f_0|}\sqrt{\beta/U-k^2}.
$$

The unique outgoing forced component is then

$$
\boxed{\psi'(x,z)=\frac{N^2b_0}{f_0m}\cos(kx+mz),\qquad
\sigma'=-N^2b_0\sin(kx+mz),\qquad
w'=Ukb_0\cos(kx+mz).}
$$

The bottom derivative and $w'(0)=Ub_x$ verify the phase and amplitude. In this stationary pattern it is the intrinsic frequency $\omega_{\mathrm{int}}=-Uk$ that describes downward vertical phase propagation relative to the current; the laboratory frequency is zero.

If $U<0$ or $U>\beta/k^2$, define

$$
\lambda=\frac N{|f_0|}\sqrt{k^2-\beta/U}>0.
$$

Exclude exponential growth at infinity. The unique decaying forced component is

$$
\boxed{\psi'(x,z)=\frac{N^2b_0}{f_0\lambda}e^{-\lambda z}\sin kx,\qquad
\sigma'=-N^2b_0e^{-\lambda z}\sin kx,\qquad
w'=Ukb_0e^{-\lambda z}\cos kx.}
$$

At the excluded value $U=\beta/k^2$, a nonzero prescribed bottom derivative cannot be matched by a bounded constant/linear vertical solution; the steady idealization is singular. At $U=0$ the boundary is not crossed and there is no forced response in the linear nonzero-$k$ sector: $\psi'=0$, rather than an expression obtained by dividing by $U$. Uniqueness throughout refers to the prescribed forced Fourier component, with the reference state fixed and no independently incident waves or added mean-state changes.

The propagation criterion explains why topographically forced planetary [Rossby waves](../../../../../rossby-wave.md) can carry energy into a moderately westerly stratosphere, while easterlies and sufficiently strong westerlies block their vertical propagation. Larger horizontal scales more readily meet the criterion. Real dissipation, height-dependent winds and critical levels modify the simple solution and allow wave–mean-flow interaction; the ideal constant-coefficient calculation establishes the propagation filter, not a complete theory of stratospheric evolution.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

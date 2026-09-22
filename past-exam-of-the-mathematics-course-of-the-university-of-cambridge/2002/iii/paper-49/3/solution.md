<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The basic [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) $\bar\psi=-\Lambda yz$ gives $\bar u=\Lambda z$, $\bar v=0$ and constant [quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) $\bar Q=f$. Define

$$
q'=\nabla_h^2\psi'+\frac{f^2}{N^2}\psi'_{zz}.
$$

Because the background has no [potential-vorticity gradient](../../../../../potential-vorticity-gradient.md), the linear [potential-vorticity equation](../../../../../potential-vorticity-evolution-equation.md) is simply

$$
(\partial_t+\Lambda z\partial_x)q'=0.
$$

Its [characteristics](../../../../../characteristic-of-a-field.md) have constant $y,z,x-\Lambda zt$, so the general solution is $q'=\mathcal F(y,z,x-\Lambda zt)$. In particular, $q'=F(y,z)G(x-\Lambda zt)$ is the requested arbitrary separated family; one product is not the most general initial field.

Linearizing the vertical [velocity](../../../../../velocity.md) requires retaining advection of $\bar\psi_z=-\Lambda y$ by $v'=\psi'_x$. Therefore

$$
w'=-\frac f{N^2}\left[(\partial_t+\Lambda z\partial_x)\psi'_z-\Lambda\psi'_x\right].
$$

The impermeable boundary at $z=0$ imposes

$$
\boxed{\partial_t\psi'_z-\Lambda\psi'_x=0\quad(z=0).}
$$

This is conservation of boundary [buoyancy](../../../../../buoyancy.md), not merely a condition that $\psi'_z$ vanish.

For zero interior [potential vorticity](../../../../../potential-vorticity.md), write $\psi'=\operatorname{Re}\{\phi(z,t)e^{i(kx+ly)}\}$. With $K_h=\sqrt{k^2+l^2}>0$, [stratified quasi-geostrophic inversion](../../../../../stratified-quasi-geostrophic-inversion.md) gives

$$
\phi_{zz}-\frac{N^2K_h^2}{f^2}\phi=0.
$$

The decaying solution is

$$
\boxed{\phi=A(t)e^{-\mu z},\qquad\mu=\frac{N K_h}{f}.}
$$

No time dependence has been assumed to obtain this vertical structure. Applying the boundary condition gives $-\mu\dot A-i\Lambda kA=0$, hence

$$
\boxed{A=A_0e^{-i\omega t},\qquad
\omega=\frac{\Lambda k}{\mu}=\frac{f\Lambda k}{N\sqrt{k^2+l^2}}.}
$$

Thus the [Eady edge wave](../../../../../eady-edge-wave.md) travels eastward with [horizontal phase velocity](../../../../../horizontal-phase-velocity.md) $\omega/k=\Lambda/\mu$ for $k\ne0$.

The propagation mechanism can be made explicit using boundary parcels. [Thermal wind](../../../../../thermal-wind.md) gives the background [buoyancy gradient](../../../../../buoyancy-gradient.md) $\bar b_y=f\bar\psi_{zy}=-f\Lambda$. A small meridional parcel [displacement](../../../../../displacement.md) $d$ produces boundary [buoyancy perturbation](../../../../../buoyancy-perturbation.md) $b'=-d\bar b_y=f\Lambda d$. Meanwhile the decaying [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) gives $b'=f\psi'_z=-f\mu\psi'$ at the boundary. Consequently $\psi'=-\Lambda d/\mu$ there, and the parcel equation $d_t=v'=\psi'_x$ becomes

$$
d_t+\frac\Lambda\mu d_x=0.
$$

A displaced buoyancy contour therefore induces a [velocity field](../../../../../velocity-field.md) that advances that displacement eastward. No interior [potential-vorticity gradient](../../../../../potential-vorticity-gradient.md) is needed because the boundary buoyancy supplies the invertibility data.

[Vortex stretching](../../../../../vortex-stretching.md) is what sets the induced flow's vertical reach. In the interior, the zero-[potential vorticity](../../../../../potential-vorticity.md) condition requires

$$
\underbrace{\nabla_h^2\psi'}_{\text{relative vorticity}}=-K_h^2\psi',\qquad
\underbrace{\frac{f^2}{N^2}\psi'_{zz}}_{\text{stretching}}=+K_h^2\psi'.
$$

Boundary [isopycnal displacement](../../../../../isopycnal-displacement.md) decreases with height as $e^{-\mu z}$, so fluid columns are stretched or compressed over depth $\mu^{-1}=f/(NK_h)$. Conservation of [potential vorticity](../../../../../potential-vorticity.md) makes this stretching balance the [relative vorticity](../../../../../relative-vorticity.md). The resulting inversion factor $b'=-f\mu\psi'$ gives the propagation speed: stronger [density stratification](../../../../../density-stratification.md) reduces penetration and speed, while larger $f$ increases them. Zero interior [potential vorticity](../../../../../potential-vorticity.md) therefore does not imply zero interior flow.

For imposed boundary vertical [velocity](../../../../../velocity.md), retain the same decaying structure and write

$$
w'(0)=\operatorname{Re}\{\epsilon e^{i(kx+ly-\omega_0t)}\}.
$$

The boundary relation becomes the [forced Eady edge wave](../../../../../forced-eady-edge-wave.md) equation

$$
\dot A+i\omega A=C e^{-i\omega_0t},\qquad C=\frac{N^2\epsilon}{f\mu}.
$$

The [integrating factor](../../../../../integrating-factor.md) $e^{i\omega t}$ gives, for $\omega_0\ne\omega$,

$$
\boxed{A(t)=B e^{-i\omega t}+\frac{C}{i(\omega-\omega_0)}e^{-i\omega_0t},\qquad
\psi'=\operatorname{Re}\{A(t)e^{-\mu z+i(kx+ly)}\}.}
$$

The arbitrary homogeneous coefficient $B$ sets the initial disturbance. With $A(0)=0$, this is $A=C(e^{-i\omega_0t}-e^{-i\omega t})/[i(\omega-\omega_0)]$.

At [resonance](../../../../../resonance.md), $\omega_0=\omega$, integration instead yields

$$
\boxed{A(t)=(B+Ct)e^{-i\omega t}.}
$$

An initially undisturbed fluid has $\psi'=Ct e^{-\mu z}\cos(kx+ly-\omega t)$. The imposed pumping reinforces the same boundary [normal mode](../../../../../normal-mode.md) every cycle, with no dissipative loss, so the linear amplitude grows secularly. The divergence describes [resonance](../../../../../resonance.md) of the undamped linear model; sufficiently large [wave amplitude](../../../../../wave-amplitude.md) invalidates the assumed small-disturbance approximation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $L$ be a core-scale length, $B_*$ a representative strength of the prescribed [poloidal magnetic field](../../../../../poloidal-magnetic-field.md), and $v_A=B_*/\sqrt{\mu_0\rho}$ the [Alfvén speed](../../../../../alfven-speed.md). A consistent weakly damped, small-amplitude ordering is

$$
\frac{v_A}{\Omega L}\ll1,\qquad U\ll v_A,\qquad
\frac{|\mathbf u_p|}{L}\ll\sigma\sim\frac{v_A}{L},\qquad
\frac{\nu}{L^2},\frac{\eta}{L^2}\ll\sigma.
$$

The first ratio is the [Lehnert number](../../../../../lehnert-number.md). It makes the wave slow relative to rotation and allows almost [geostrophic flow](../../../../../geostrophic-flow.md), with the azimuthal velocity approximately constant along a rotation-axis cylinder. The small wave amplitude gives $|B_\phi|\sim\sqrt{\mu_0\rho}|U|\ll B_*$. Poloidal advection then changes neither the background field nor the wave substantially over one wave period. If there are no-slip boundary layers, also require their damping rate $\sqrt{\nu\Omega}/L\ll\sigma$, or otherwise retain their torque; a small bulk viscosity alone does not remove that boundary torque.

In the rotating [magnetohydrodynamic momentum equation](../../../../../magnetohydrodynamic-momentum-equation.md), axisymmetry removes the azimuthal pressure derivative. The neglected nonlinear azimuthal advection has size $|\mathbf u_p|U/L$, and the neglected viscous term has size $\nu U/L^2$. The retained azimuthal [Coriolis force](../../../../../coriolis-force.md) is $2\Omega u_r$. A typical compatible local balance has $|u_r|\sim\sigma U/\Omega$, small compared with $U$ when the [Lehnert number](../../../../../lehnert-number.md) is small. The azimuthal [Lorentz force density](../../../../../lorentz-force-density.md) can be written using $\nabla\cdot\mathbf B_p=0$:

$$
\frac{1}{\mu_0\rho}\left(\mathbf B_p\cdot\nabla B_\phi+\frac{B_rB_\phi}{r}\right)
=\frac{1}{\mu_0\rho r}\nabla\cdot(r\mathbf B_pB_\phi).
$$

The physical prefactor is $1/(\mu_0\rho)$: the extra $i$ printed inside the first reduced momentum equation is a typographical error, also contradicted by the subsequent real-valued system.

In the [resistive induction equation](../../../../../resistive-induction-equation.md), neglecting poloidal advection of the perturbation and magnetic diffusion leaves the winding of the prescribed [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) by differential rotation. Thus

$$
U_t+2\Omega u_r=\frac{1}{\mu_0\rho r}\nabla\cdot(r\mathbf B_pB_\phi),\qquad
(B_\phi)_t=r\mathbf B_p\cdot\nabla(U/r).
$$

This is the small-amplitude [torsional Alfvén wave](../../../../../torsional-alfven-wave.md) approximation, with a time-independent background and no external azimuthal forcing.

We now average over the full height of a rotation-axis cylinder. The sphere is impenetrable. Integrating [incompressible flow](../../../../../incompressible-flow.md) over the volume inside any such cylinder gives zero flux through its cylindrical side, since there is no flux through its spherical caps. Therefore

$$
\int_{-z_b}^{z_b}u_r\,dz=0.
$$

This is why the [Coriolis force](../../../../../coriolis-force.md) disappears from the cylinder average; it need not vanish locally. An axisymmetric field in the insulating exterior is a potential field with $B_\phi=0$, so continuity gives $B_\phi=0$ on the sphere. Consequently both the end flux terms and the moving-endpoint terms in the magnetic-stress integral vanish. Expanding the divergence gives

$$
\frac1r\nabla\cdot(r\mathbf B_pB_\phi)
=\frac1{r^2}\partial_r(r^2B_rB_\phi)+\partial_z(B_zB_\phi).
$$

Since $U$ is independent of $z$, its integrated time derivative is $2z_bU_t$. Defining $T=\int_{-z_b}^{z_b}B_rB_\phi\,dz$ gives

$$
\boxed{U_t=\frac{1}{2z_b\mu_0\rho r^2}\partial_r(r^2T).}
$$

The stationary background and the fact that $U/r$ depends only on $r,t$ also give

$$
T_t=\int_{-z_b}^{z_b}B_r(B_\phi)_t\,dz
=r\partial_r(U/r)\int_{-z_b}^{z_b}B_r^2\,dz,
$$

so

$$
\boxed{T_t=H(r)r\partial_r(U/r),\qquad H(r)=\int_{-z_b}^{z_b}B_r^2\,dz.}
$$

Together these form the [cylinder-averaged torsional Alfvén wave](../../../../../cylinder-averaged-torsional-alfven-wave.md) system.

Assume $H>0$ on the cylinders carrying the wave, with regular endpoint limits. If $H$ vanishes on an interior cylinder, then $B_r$ and $T$ vanish there and that cylinder has no radial magnetic coupling; the displayed $H^{-1}$ energy term must be interpreted on the coupled region rather than literally dividing by zero. Since $H$ is time independent, differentiation of the proposed [conserved energy of a cylinder-averaged torsional wave](../../../../../conserved-energy-of-a-cylinder-averaged-torsional-wave.md) gives

$$
\begin{aligned}
\frac{dE}{dt}
&=\int_0^a\left(2z_b\mu_0\rho U U_t+\frac{T}{H}T_t\right)r\,dr\\
&=\int_0^a\left[\frac Ur\partial_r(r^2T)+r^2T\partial_r(U/r)\right]dr\\
&=[rUT]_0^a=0.
\end{aligned}
$$

Regularity at the rotation axis makes the lower endpoint vanish, while vanishing magnetic torque at the collapsed outer cylinder makes the upper endpoint vanish. This proves

$$
\boxed{E=\frac12\int_0^a\left(2z_b\mu_0\rho U^2+\frac{T^2}{H}\right)r\,dr\quad\text{is conserved}.}
$$

The magnetic term has a direct interpretation. Decompose $B_\phi=(T/H)B_r+B_\phi^\perp$, with $\int B_rB_\phi^\perp\,dz=0$. Then $\int B_\phi^2\,dz=T^2/H+\int(B_\phi^\perp)^2\,dz$, and the induction equation gives $(B_\phi^\perp)_t=0$. Thus, apart from a common dimensional factor and a stationary orthogonal magnetic component, the conserved quantity is the physical kinetic plus [magnetic energy](../../../../../magnetic-energy.md).

For the frequency estimate, put $V=U/r$ and eliminate $T$:

$$
V_{tt}=\frac{1}{2z_b\mu_0\rho r^3}\partial_r(r^3H V_r).
$$

Locally this is a [wave equation](../../../../../wave-equation-split.md) with speed

$$
\boxed{c_T(r)=\sqrt{\frac{H(r)}{2z_b(r)\mu_0\rho}}=\frac{\sqrt{\langle B_r^2\rangle_z}}{\sqrt{\mu_0\rho}}.}
$$

It is the cylinder-averaged radial field component that matters, not simply the dipole measured at the Earth's surface. Taking a cylinder height of order $6\times10^6\,\mathrm m$, $\rho\sim10^4\,\mathrm{kg\,m^{-3}}$, and an assumed internal cylindrical radial field $B_{r,\mathrm{rms}}\sim0.2$--$2\,\mathrm{mT}$ gives

$$
H\sim0.2\text{--}20\,\mathrm{T^2\,m},\qquad c_T\sim2\times10^{-3}\text{--}2\times10^{-2}\,\mathrm{m\,s^{-1}}.
$$

For a standing wave of radial length $L_c\sim2$--$3.5\times10^6\,\mathrm m$, the cyclic frequency is of order $c_T/(2L_c)$ and the angular frequency is of order $\pi c_T/L_c$. Hence

$$
\boxed{\nu_T\sim10^{-10}\text{--}10^{-9}\,\mathrm{Hz},\qquad\text{periods of order years to a century}.}
$$

Geometry and the assumed internal field can shift the estimate substantially. As a concrete calibration, [the 2010 torsional-wave study](https://www.nature.com/articles/nature09010) inferred a cylindrical radial rms field near $2\,\mathrm{mT}$ and a roughly four-year crossing time, with an observed six-year recurrence. A much weaker assumed interior field instead gives the older multi-decadal estimate. The paper supplies no numerical interior field strength, so a unique numerical frequency cannot be deduced without such an assumption.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose a reference [circular orbit](../../../../../circular-orbit.md) at radius $r_0$, rotate the frame with $\boldsymbol\Omega=\Omega(r_0)\mathbf e_z$, and introduce local Cartesian coordinates $x=r-r_0$, $y=r_0(\phi-\Omega t)$ and vertical coordinate $z$. On scales small compared with $r_0$, neglect curvature of the coordinate directions but retain the leading [differential rotation](../../../../../differential-rotation.md). The background [velocity](../../../../../velocity.md) relative to the rotating frame is

$$
\mathbf u_0=r_0\Omega'(r_0)x\mathbf e_y=-2Ax\mathbf e_y,\qquad A=-\frac12r_0\Omega'(r_0).
$$

Thus $A=3\Omega/4$ for a [Keplerian disk](../../../../../keplerian-disk.md). The [shearing sheet](../../../../../shearing-sheet.md) retains [Coriolis acceleration](../../../../../coriolis-acceleration.md) and the linear tidal acceleration. The radial [shearing-sheet tidal potential](../../../../../shearing-sheet-tidal-potential.md) is $-2\Omega Ax^2$, whose force $4\Omega Ax\mathbf e_x$ balances the background [Coriolis acceleration](../../../../../coriolis-acceleration.md). If vertical tidal gravity is included, its equilibrium contribution is balanced by a background [pressure](../../../../../pressure.md) $p_0(z)$ and disappears when that equilibrium is subtracted.

Write the total [velocity](../../../../../velocity.md) as $\mathbf u=\mathbf u_0+\mathbf v$. In the rotating-frame [magnetohydrodynamic momentum equation](../../../../../magnetohydrodynamic-momentum-equation.md), background advection is $(\mathbf u_0\cdot\nabla)\mathbf v=-2Ax\partial_y\mathbf v$ and advection of the background by the perturbation is $(\mathbf v\cdot\nabla)\mathbf u_0=-2Av_x\mathbf e_y$. The uniform-viscosity [diffusion](../../../../../diffusion.md) of the linear background shear is zero. For a solenoidal [magnetic field](../../../../../magnetic-field.md) the [Lorentz force](../../../../../lorentz-force.md) per unit [mass](../../../../../mass.md) is

$$
\frac{(\nabla\times\mathbf B)\times\mathbf B}{\mu_0\rho}=\frac{\mathbf B\cdot\nabla\mathbf B}{\mu_0\rho}-\nabla\frac{B^2}{2\mu_0\rho}.
$$

At constant [density](../../../../../density.md), absorb the magnetic-pressure gradient into $\psi=(p-p_0)/\rho+B^2/(2\mu_0\rho)$. Subtracting the background force balance then gives the stated momentum equation, with the remaining nonlinear advection $\mathbf v\cdot\nabla\mathbf v$, [Coriolis acceleration](../../../../../coriolis-acceleration.md) $2\boldsymbol\Omega\times\mathbf v$, [magnetic tension](../../../../../magnetic-tension.md) and viscous [diffusion](../../../../../diffusion.md).

For constant finite [electrical conductivity](../../../../../electrical-conductivity.md) $\sigma_e$, put $\eta=(\mu_0\sigma_e)^{-1}$. The [resistive induction equation](../../../../../resistive-induction-equation.md) with uniform [magnetic diffusivity](../../../../../magnetic-diffusivity.md) is $\partial_t\mathbf B+\mathbf u\cdot\nabla\mathbf B=\mathbf B\cdot\nabla\mathbf u+\eta\nabla^2\mathbf B$. Substituting the background shear supplies the term $-2AB_x\mathbf e_y$ and the same background-advection operator as in the momentum equation. The two further conditions are

$$
\boxed{\nabla\cdot\mathbf v=0,\qquad\nabla\cdot\mathbf B=0.}
$$

They express [incompressibility](../../../../../incompressible-flow.md) and the absence of [magnetic monopoles](../../../../../magnetic-monopole.md), respectively.

Now take real [plane waves](../../../../../plane-wave.md) with common phase $\vartheta=\mathbf k(t)\cdot\mathbf x$ and real [wavevector](../../../../../wavevector.md). The solenoidal conditions become

$$
\mathbf k\cdot\widetilde{\mathbf v}=0,\qquad \mathbf k\cdot\widetilde{\mathbf B}=0.
$$

Every field depends on position only through $\vartheta$. Hence for either transverse [vector](../../../../../vector.md) field $\mathbf P$ and either wave field $\mathbf Q$, $(\mathbf P\cdot\nabla)\mathbf Q=(\mathbf P\cdot\mathbf k)\partial_\vartheta\mathbf Q=0$. This proves that all the displayed quadratic advection and tension terms vanish pointwise, including products involving conjugate [amplitudes](../../../../../wave-amplitude.md). These waves are therefore exact solutions at finite [amplitude](../../../../../wave-amplitude.md), not merely a [linearization](../../../../../linearization.md).

Acting with $D_0=\partial_t-2Ax\partial_y$ on the phase yields

$$
D_0\vartheta=(\dot k_x-2Ak_y)x+\dot k_y y+\dot k_z z.
$$

Canceling its position-dependent part requires

$$
\boxed{\dot k_x=2Ak_y,\qquad\dot k_y=\dot k_z=0,\qquad k_x(t)=k_{x0}+2Ak_yt.}
$$

The remaining [amplitude](../../../../../wave-amplitude.md) equations are

$$
\boxed{\dot{\widetilde{\mathbf v}}-2A\widetilde v_x\mathbf e_y+2\boldsymbol\Omega\times\widetilde{\mathbf v}=-i\mathbf k\widetilde\psi-\nu k^2\widetilde{\mathbf v},\qquad\dot{\widetilde{\mathbf B}}=-2A\widetilde B_x\mathbf e_y-\eta k^2\widetilde{\mathbf B}.}
$$

Differentiating the [velocity](../../../../../velocity.md) constraint determines the [pressure](../../../../../pressure.md) [amplitude](../../../../../wave-amplitude.md):

$$
i k^2\widetilde\psi=4Ak_y\widetilde v_x-2\mathbf k\cdot(\boldsymbol\Omega\times\widetilde{\mathbf v}).
$$

The [resistive induction equation](../../../../../resistive-induction-equation.md) preserves its constraint because $\dot{\mathbf k}\cdot\widetilde{\mathbf B}=2Ak_y\widetilde B_x$ cancels the corresponding shear term in $\mathbf k\cdot\dot{\widetilde{\mathbf B}}$. The specified [magnetic field](../../../../../magnetic-field.md) has no spatially uniform part. Thus there is no background [magnetic field](../../../../../magnetic-field.md) producing an additional linear magnetic-tension coupling. The scalar $\psi$ is the modified [pressure](../../../../../pressure.md); the physical [pressure](../../../../../pressure.md) can include a constant and a second spatial harmonic from $-B^2/(2\mu_0)$ while $\psi$ retains the stipulated plane-wave form. This is an exact [zero-mean magnetic shearing wave](../../../../../zero-mean-magnetic-shearing-wave.md).

For decay, take the real part of the [scalar product](../../../../../dot-product.md) of the velocity-amplitude equation with its [complex conjugate](../../../../../complex-conjugate.md). [Pressure](../../../../../pressure.md) does no work because $\mathbf k\cdot\widetilde{\mathbf v}=0$, and the real part of Coriolis work is zero. Therefore

$$
\frac{d}{dt}|\widetilde{\mathbf v}|^2=4A\operatorname{Re}(\widetilde v_x\widetilde v_y^*)-2\nu k^2|\widetilde{\mathbf v}|^2\le(2|A|-2\nu k^2)|\widetilde{\mathbf v}|^2.
$$

The [resistive induction equation](../../../../../resistive-induction-equation.md) similarly gives

$$
\frac{d}{dt}|\widetilde{\mathbf B}|^2=-4A\operatorname{Re}(\widetilde B_x\widetilde B_y^*)-2\eta k^2|\widetilde{\mathbf B}|^2\le(2|A|-2\eta k^2)|\widetilde{\mathbf B}|^2,
$$

using $2|u_xu_y|\le|\mathbf u|^2$. Integrating these differential inequalities, define

$$
J(t)=\int_0^t k(s)^2\,ds=(k_{x0}^2+k_y^2+k_z^2)t+2Ak_{x0}k_yt^2+\frac43A^2k_y^2t^3.
$$

Then

$$
|\widetilde{\mathbf v}(t)|^2\le|\widetilde{\mathbf v}(0)|^2e^{2|A|t-2\nu J(t)},\qquad |\widetilde{\mathbf B}(t)|^2\le|\widetilde{\mathbf B}(0)|^2e^{2|A|t-2\eta J(t)}.
$$

A non-axisymmetric wave has $k_y\ne0$. For nonzero differential shear and positive $\nu,\eta$, the negative cubic terms dominate the linear upper bound on shear work. Consequently

$$
\boxed{\widetilde{\mathbf v}(t)\longrightarrow0,\qquad\widetilde{\mathbf B}(t)\longrightarrow0\quad(t\to\infty).}
$$

This [cubic-exponent decay of a nonaxisymmetric shearing wave](../../../../../cubic-exponent-decay-of-a-nonaxisymmetric-shearing-wave.md) allows transient [energy](../../../../../energy.md) growth before the winding to short radial wavelengths makes [diffusion](../../../../../diffusion.md) dominant. The magnetic [amplitudes](../../../../../wave-amplitude.md) can also be written explicitly as

$$
\widetilde{\mathbf B}(t)=e^{-\eta J(t)}\big(\widetilde B_x(0),\ \widetilde B_y(0)-2At\widetilde B_x(0),\ \widetilde B_z(0)\big),
$$

which confirms the damping independently. Positivity of the dissipative coefficients is necessary: with $k_z=0$, an inviscid vertical [velocity](../../../../../velocity.md) [amplitude](../../../../../wave-amplitude.md) can remain constant, and an ideal vertical magnetic [amplitude](../../../../../wave-amplitude.md) can remain constant when $\eta=0$. The asserted decay applies to the viscous, finitely conducting model; taking an ideal limit before the long-time limit changes the conclusion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

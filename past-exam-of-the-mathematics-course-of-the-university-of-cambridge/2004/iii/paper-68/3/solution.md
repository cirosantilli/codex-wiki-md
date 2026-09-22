<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The additional conditions are **$\boxed{\nabla\cdot\mathbf u=0,\qquad\nabla\cdot\mathbf B=0}$**: [incompressible flow](../../../../../incompressible-flow.md) and the solenoidal [magnetic field](../../../../../magnetic-field.md) constraint. The scalar $\Psi$ combines pressure per unit density with [magnetic pressure](../../../../../magnetic-pressure.md) per unit density and any conservative gravitational and centrifugal potentials. In particular, the [Lorentz force](../../../../../lorentz-force.md) identity separates magnetic tension from $-\nabla(B^2/2\mu_0\rho)$. Adding this latter term to the [rotating-flow pressure potential](../../../../../rotating-flow-pressure-potential.md) gives the pressure appearing in the stated equation; the [Coriolis force](../../../../../coriolis-force.md) remains explicit.

Work in magnetic velocity units $\mathbf B/\sqrt{\mu_0\rho}$, and write $\mathbf U=-2Ax\mathbf e_y$ for the background [shearing sheet](../../../../../shearing-sheet.md) flow. Its advective acceleration is zero, and $2\Omega\mathbf e_z\times\mathbf U=4\Omega Ax\mathbf e_x=-\nabla(-2\Omega Ax^2)$, so the stated quadratic background pressure potential gives an exact balance. A spatially uniform mean magnetic field must evolve as

$$
\boxed{\dot{\bar{\mathbf b}}=-2A\bar b_x\mathbf e_y,\qquad \bar b_x,\bar b_z=\mathrm{constant},\qquad\bar b_y(t)=\bar b_y(0)-2A\bar b_x t.}
$$

This is stretching of radial field into azimuthal field by [differential rotation](../../../../../differential-rotation.md).

For the [shearing wave](../../../../../shearing-wave.md) phase $\Theta=\mathbf k(t)\cdot\mathbf x$, advection by the background gives

$$
(\partial_t+\mathbf U\cdot\nabla)\Theta=\dot{\mathbf k}\cdot\mathbf x-2Axk_y.
$$

It vanishes identically if

$$
\boxed{\dot{\mathbf k}=2Ak_y\mathbf e_x,\qquad k_x(t)=k_x(0)+2Ak_yt,\qquad k_y,k_z=\mathrm{constant}.}
$$

The changing wavevector describes the shear of initially planar wavefronts. The mean-field stretching and wavevector evolution cancel in the [Alfvén frequency](../../../../../alfven-frequency.md):

$$
\frac{d}{dt}(\mathbf k\cdot\bar{\mathbf b})=2Ak_y\bar b_x-2Ak_y\bar b_x=0.
$$

Hence **$\boxed{\omega_A=\mathbf k\cdot\bar{\mathbf b}\ \text{is constant}}$**.

These solutions are exact finite-amplitude disturbances, not merely a linearization. To see this, let $\mathbf u'=\operatorname{Re}(\mathbf ve^{i\Theta})$ and $\mathbf B'=\operatorname{Re}(\mathbf be^{i\Theta})$ in magnetic velocity units. The divergence constraints give $\mathbf k\cdot\mathbf v=\mathbf k\cdot\mathbf b=0$. Thus both real disturbances are pointwise perpendicular to k, whereas all their spatial derivatives are along k. Every quadratic term $\mathbf u'\cdot\nabla\mathbf u'$, $\mathbf B'\cdot\nabla\mathbf B'$, $\mathbf u'\cdot\nabla\mathbf B'$ and $\mathbf B'\cdot\nabla\mathbf u'$ vanishes, including terms involving conjugate amplitudes. This extends the [exact incompressible shearing wave](../../../../../exact-incompressible-shearing-wave.md) to an [exact magnetic shearing wave](../../../../../exact-magnetic-shearing-wave.md). The gas pressure can compensate quadratic magnetic-pressure terms even though the combined $\Psi$ contains only its stated background and wave harmonic.

The remaining wave terms are therefore precisely

$$
\boxed{\begin{aligned}
\dot{\mathbf v}-2Av_x\mathbf e_y+2\Omega\mathbf e_z\times\mathbf v&=-i\mathbf k\psi+i\omega_A\mathbf b-\nu k^2\mathbf v,\\
\dot{\mathbf b}&=-2Ab_x\mathbf e_y+i\omega_A\mathbf v-\eta k^2\mathbf b,\\
\mathbf k\cdot\mathbf v&=\mathbf k\cdot\mathbf b=0.
\end{aligned}}
$$

The shear terms arise from perturbations acting on $\nabla\mathbf U$, the magnetic terms from the uniform field acting on the wave, and the last terms from diffusion. Pressure enforces the moving-wavevector velocity constraint: differentiating it gives

$$
i k^2\psi=4Ak_yv_x-2\Omega\mathbf k\cdot(\mathbf e_z\times\mathbf v).
$$

Using this pressure leaves $\mathbf k\cdot\mathbf v=0$ invariant. Differentiating $\mathbf k\cdot\mathbf b$ in the induction equation similarly leaves it zero. Thus the evolution is consistent with both constraints for initially transverse amplitudes.

Now take positive $\Omega$, so the stipulated condition implies $0<A<2\Omega$, and take [magnetic Prandtl number](../../../../../magnetic-prandtl-number.md) $\nu/\eta=1$, with $\nu=\eta>0$. For a vertical wavevector $\mathbf k=k\mathbf e_z$, use the [equal-diffusivity magnetorotational channel](../../../../../equal-diffusivity-magnetorotational-channel.md) form

$$
\mathbf v=(V,V,0),\qquad\mathbf b=(B,-B,0),\qquad\psi=0.
$$

The two horizontal momentum equations, after adding them, give $\dot V=(A-\nu k^2)V$. Either component then gives $i\omega_AB=(A-2\Omega)V$. The first induction equation gives $(\partial_t+\nu k^2)B=i\omega_AV$. These equations are simultaneously solved by

$$
\boxed{\omega_A^2=A(2\Omega-A),\qquad B=\frac{i\omega_A}{A}V,\qquad V(t)=V_0e^{\gamma t},\qquad\gamma=A-\nu k^2.}
$$

The second induction component gives the same relation, since $B_y=-B_x$. **Exponential growth occurs when $\boxed{\nu k^2<A}$**. The quarter-cycle phase between magnetic and velocity perturbations is required by the factor i in the Fourier equations.

For [Keplerian rotation](../../../../../keplerian-disk.md), expanding the local shear gives $2A=-(r\Omega')=3\Omega/2$, hence $A=3\Omega/4$. Therefore $\omega_A^2=15\Omega^2/16$. With $v_{Az}=\bar B_z/\sqrt{\mu_0\rho}$ and $\omega_A=kv_{Az}$, the growth condition for this prescribed polarization becomes

$$
\boxed{v_{Az}^2>\nu(2\Omega-A)=\frac54\nu\Omega,\qquad |\bar B_z|>\sqrt{\frac54\mu_0\rho\nu\Omega}.}
$$

A weaker field would require a shorter wavelength to retain this mode's selected Alfvén frequency, making diffusive damping too strong. The required wavelength must also fit any actual vertical domain; no vertical boundary conditions are specified here.

The field bound is for the requested equal-component mode, rather than a universal necessary condition for all [magnetorotational instability](../../../../../magnetorotational-instability.md). This distinction matters if all vertical wavelengths are admitted. Indeed, let $s=\gamma+\nu k^2$ for a general horizontal polarization. Eliminating its two magnetic amplitudes gives $(s+\omega_A^2/s)v_x-2\Omega v_y=0$ and $(s+\omega_A^2/s)v_y+[2(\Omega-A)-2A\omega_A^2/s^2]v_x=0$. Their determinant gives

$$
(s^2+\omega_A^2)^2+\kappa^2s^2-4\Omega A\omega_A^2=0,\qquad\kappa^2=4\Omega(\Omega-A).
$$

For a [Keplerian disk](../../../../../keplerian-disk.md), $\kappa^2=\Omega^2$. As a concrete counterexample to a universal reading of the bound, in consistent dimensionless units take $\Omega=1$, $A=3/4$, $\nu=\eta=1$, $v_{Az}=0.1$, and $k=0.01$. The positive root gives $s\simeq0.00173205$ and $\gamma=s-0.0001>0$, even though $v_{Az}^2=0.01<1.25$. This mode has a different polarization and a much longer wavelength. Real finite-height discs restrict such wavelengths; the PDF supplies no such restriction.

Finally, the horizontally averaged radial flux of azimuthal momentum is the sum of [Reynolds stress](../../../../../reynolds-stress.md) and magnetic tension stress:

$$
T_{xy}=\rho\langle u'_xu'_y\rangle-\frac1{\mu_0}\langle B'_xB'_y\rangle=\frac\rho2(|V|^2+|B|^2)>0.
$$

Multiplication by the local radius gives an outward angular-momentum flux. Equal radial and azimuthal velocities give the largest positive product at fixed horizontal kinetic energy, while opposite magnetic components give the largest positive $-B_xB_y$ at fixed horizontal magnetic energy. Both follow from $2|ab|\leq|a|^2+|b|^2$. This [stress-maximizing magnetorotational channel polarization](../../../../../stress-maximizing-magnetorotational-channel-polarization.md) therefore makes both contributions reinforce outward [angular momentum transport](../../../../../angular-momentum-transport.md). It extracts shear energy at rate $-T_{xy}\partial_xU_y=2AT_{xy}>0$, explaining why these correlations are especially effective in driving accretion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

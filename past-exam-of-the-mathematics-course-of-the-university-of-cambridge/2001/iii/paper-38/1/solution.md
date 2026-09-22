<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work with the complex representation and take its real part to obtain the physical [magnetic field](../../../../../magnetic-field.md). For constant [magnetic diffusivity](../../../../../magnetic-diffusivity.md) and the prescribed circular [velocity](../../../../../velocity.md) $\mathbf u=s\Omega(s)\widehat{\boldsymbol\phi}$, the [resistive induction equation](../../../../../resistive-induction-equation.md) and $\mathbf B=\nabla\times(A\widehat{\mathbf z})$ give

$$
B_s=\frac1s\partial_\phi A,\qquad B_\phi=-\partial_s A,\qquad
\partial_tA+\Omega\partial_\phi A=\eta\left(\partial_s^2A+\frac1s\partial_sA+\frac1{s^2}\partial_\phi^2A\right).
$$

To see the last equation directly, $\mathbf u\times\mathbf B=-s\Omega B_s\widehat{\mathbf z}=-\Omega A_\phi\widehat{\mathbf z}$. Taking its [curl](../../../../../curl.md) reproduces the induction equation if $A_t=-\Omega A_\phi+\eta\nabla^2A$, up to a time-dependent additive constant removable by the [gauge transformation](../../../../../gauge-transformation.md). This is the scalar form of advection and [magnetic diffusion](../../../../../magnetic-diffusion.md) in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md).

Put $\psi=\phi-\Omega(s)t$. The [material derivative](../../../../../material-derivative.md) of $ae^{i\psi}$ is $a_t e^{i\psi}$, because $\psi_t+\Omega\psi_\phi=0$. A radial [derivative](../../../../../derivative.md) instead acts on both amplitude and phase:

$$
\partial_sA=(a_s-it\Omega'a)e^{i\psi},\qquad
\partial_s^2A=(a_{ss}-2it\Omega'a_s-it\Omega''a-t^2(\Omega')^2a)e^{i\psi}.
$$

Also $A_{\phi\phi}=-ae^{i\psi}$. Substitution gives the [shearing-coordinate magnetic flux equation](../../../../../shearing-coordinate-magnetic-flux-equation.md), here for azimuthal mode number one:

$$
\boxed{a_t=\eta\left[a_{ss}+\frac{a_s}{s}-\frac a{s^2}-(\Omega')^2t^2a-2it\Omega'a_s-\frac{it\Omega'}s a-it\Omega''a\right].}
$$

Writing it with $a_t$ on the left is important when considering zero [magnetic diffusivity](../../../../../magnetic-diffusivity.md): one must not literally divide by $\eta=0$. **In the ideal limit, $a_t=0$**, so $A(s,\phi,t)=A(s,\phi-\Omega(s)t,0)$. This is [magnetic flux freezing](../../../../../magnetic-flux-freezing.md): the scalar flux pattern is carried with each rotating fluid ring. It does not make the [magnetic field](../../../../../magnetic-field.md) stationary. Indeed,

$$
B_s=\frac{ia(s,0)}s e^{i\psi},\qquad B_\phi=[-a_s(s,0)+it\Omega'a(s,0)]e^{i\psi},
$$

so [differential rotation](../../../../../differential-rotation.md) winds the field and can make its azimuthal component grow linearly in time. Rigid rotation, for which $\Omega'=0$, only rotates the pattern.

For the specified interior [angular velocity](../../../../../angular-velocity.md), $\Omega'=-\Omega_0/d$ and $\Omega''=0$ away from the circulation edge. Let $T=\Omega_0t$, $x=s/d$ and $\mathrm{Rm}=\Omega_0d^2/\eta$. The amplitude equation becomes

$$
\partial_Ta=\frac1{\mathrm{Rm}}\left[a_{xx}+\frac{a_x}{x}-\frac a{x^2}-T^2a+2iTa_x+\frac{iT}{x}a\right].
$$

For a smooth initial amplitude on the cell scale, at $x$ bounded away from zero and the edge, the $-T^2a$ term dominates when $T\gg1$. Its accumulated damping is order one at $T=O(\mathrm{Rm}^{1/3})$, whereas the integrated terms proportional to $T$ are only $O(\mathrm{Rm}^{-1/3})$ and the terms independent of $T$ are $O(\mathrm{Rm}^{-2/3})$. The resulting [cubic-time resistive damping in a differentially rotating cell](../../../../../cubic-time-resistive-damping-in-a-differentially-rotating-cell.md) is

$$
a(s,t)\simeq a(s,0)\exp\left[-\frac{\eta\Omega_0^2t^3}{3d^2}\right],\qquad
\boxed{\tau_c=\left(\frac{3d^2}{\eta\Omega_0^2}\right)^{1/3},\quad\Omega_0\tau_c=(3\mathrm{Rm})^{1/3}.}
$$

The [magnetic field](../../../../../magnetic-field.md) has this leading [exponential decay](../../../../../exponential-decay.md) envelope. Its components also contain the algebraic winding factor visible in $B_\phi$, so the claim concerns the cubic exponent, not an exact amplitude with no prefactor. Equivalently the radial [wavenumber](../../../../../wavenumber.md) grows as $|k_s|\simeq|\Omega'|t$ and the integrated resistive damping is $\int_0^t\eta k_s^2dt=\eta(\Omega')^2t^3/3$.

This is [phase mixing in magnetic flux expulsion](../../../../../phase-mixing-in-magnetic-flux-expulsion.md). The circulation creates ever finer gradients, allowing weak [magnetic diffusion](../../../../../magnetic-diffusion.md) to act much sooner than its unsheared time $t_\eta=d^2/\eta$:

$$
\Omega_0^{-1}\ll\tau_c\ll t_\eta,\qquad \frac{\tau_c}{t_\eta}=3^{1/3}\mathrm{Rm}^{-2/3}.
$$

**Rapid winding followed by resistive smoothing expels the imposed field from the cell interior.** The maintained exterior [magnetic field](../../../../../magnetic-field.md) is redistributed into a circulation-edge [boundary layer](../../../../../boundary-layer.md). The result is an interior high-[magnetic Reynolds number](../../../../../magnetic-reynolds-number.md) transient, not a uniform assertion at the axis and the nonsmooth edge, nor the exact $t\to\infty$ solution with a continuously imposed far field. The diffusion length at $\tau_c$ is $\sqrt{\eta\tau_c}/d=3^{1/6}\mathrm{Rm}^{-1/3}$, identifying where a local bulk approximation can fail. The linear profile also needs smoothing at a regular rotation axis and at $s=d$ if used as a fully smooth global flow.

In photospheric [magnetoconvection](../../../../../magnetoconvection.md), circulating and diverging [convection](../../../../../convection.md) transports weak [magnetic flux](../../../../../magnetic-flux.md) towards converging downflow regions. [Solar granulation](../../../../../solar-granulation.md) concentrates field in [intergranular lanes](../../../../../intergranular-lane.md), while larger-scale [supergranulation](../../../../../supergranulation.md) helps form the [solar magnetic network](../../../../../solar-magnetic-network.md). [Flux expulsion](../../../../../flux-expulsion.md) explains why a highly conducting [photosphere](../../../../../photosphere.md) can have relatively weak field in cell interiors and intermittent concentrations at their edges: high [electrical conductivity](../../../../../electrical-conductivity.md) delays diffusion on the original scale, but does not prevent diffusion on the fine scales created by advection. A long-lived circulation must last long enough for the expulsion time; rapidly changing cells need not reach this idealized state. Once the field becomes strong, the [Lorentz force](../../../../../lorentz-force.md) modifies the [convection](../../../../../convection.md), so this prescribed-flow calculation alone neither determines the final field strength nor describes strong-field [sunspots](../../../../../sunspot.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

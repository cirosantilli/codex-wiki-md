<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

[Electromagnetic waves](../../../../../electromagnetic-wave-split.md) drive mobile charges in a conducting medium. Their current changes both the phase and attenuation of the wave. A description in terms of a real, frequency-independent [refractive index](../../../../../refractive-index.md) is therefore generally insufficient: the material response and the propagation constant are complex and frequency dependent.

Use [phasors](../../../../../phasor.md) proportional to $e^{i(kz-\omega t)}$, with $k=k'+ik''$ and $k''\geq0$ for a passive medium. In a homogeneous, [isotropic](../../../../../isotropy.md), linear material, let $\epsilon_b$ represent the [permittivity](../../../../../permittivity-split.md) associated with bound-charge [electric polarization](../../../../../polarization-density.md), $\mu$ the [magnetic permeability](../../../../../permeability-electromagnetism.md) and $\sigma(\omega)$ the mobile-charge conductivity. The macroscopic [Maxwell equations](../../../../../maxwell-equations-split.md) give

$$
\nabla\times\mathbf E=i\omega\mathbf B,\qquad
\nabla\times\mathbf H=(\sigma-i\omega\epsilon_b)\mathbf E.
$$

For a transverse plane wave, taking another curl yields

$$
\boxed{k^2=\mu\epsilon_b\omega^2+i\mu\sigma(\omega)\omega
=\mu\omega^2\epsilon_{\rm eff}(\omega),\qquad
\epsilon_{\rm eff}=\epsilon_b+\frac{i\sigma(\omega)}\omega.}
$$

This division of the response avoids counting mobile [electrons](../../../../../electron.md) both in $\epsilon_b$ and in $\sigma$. Define the [complex refractive index](../../../../../complex-refractive-index.md) $\widetilde n=ck/\omega=n+i\kappa$. For a nonmagnetic medium, $\widetilde n^2=\epsilon_{\rm eff}/\epsilon_0$. Its real part determines the phase variation, while the positive [optical extinction coefficient](../../../../../optical-extinction-coefficient.md) $\kappa$ gives amplitude attenuation $e^{-\omega\kappa z/c}$ and intensity attenuation $e^{-2\omega\kappa z/c}$. The amplitude penetration length is

$$
\delta=\frac1{k''}=\frac c{\omega\kappa}.
$$

A simple microscopic explanation comes from the [Drude model](../../../../../drude-model.md). Let [electrons](../../../../../electron.md) of charge $-e$, mass $m$ and [number density](../../../../../number-density.md) $n_e$ move against an effectively stationary positive background. Collisions relax their mean [velocity](../../../../../velocity.md) at rate $\nu$:

$$
m(\dot{\mathbf v}+\nu\mathbf v)=-e\mathbf E,\qquad
\mathbf J=-n_ee\mathbf v.
$$

Consequently

$$
\boxed{\sigma(\omega)=\frac{n_ee^2}{m(\nu-i\omega)}
=\frac{\epsilon_0\omega_p^2}{\nu-i\omega},\qquad
\omega_p^2=\frac{n_ee^2}{m\epsilon_0}.}
$$

With a vacuum-like bound-charge background, this gives

$$
\frac{\epsilon_{\rm eff}}{\epsilon_0}
=1-\frac{\omega_p^2}{\omega(\omega+i\nu)}.
$$

Its imaginary part is positive for positive $\omega,\nu$, consistent with dissipation under the chosen [phasor](../../../../../phasor.md) convention. Real materials can require an effective [electron](../../../../../electron.md) mass, a nontrivial bound-charge response, or additional absorption associated with the [electronic band structure](../../../../../electronic-band-structure.md).

A [plasma](../../../../../plasma-physics.md) is a conducting ionized medium with mobile [electrons](../../../../../electron.md) and [ions](../../../../../ion.md), approximately neutral on large scales because of [plasma screening](../../../../../plasma-screening.md). For the electron-frequency transverse waves considered here, the heavy [ions](../../../../../ion.md) can often be treated as stationary. In a dilute weakly collisional [plasma](../../../../../plasma-physics.md), $\nu\ll\omega$, so

$$
\boxed{n^2=1-\frac{\omega_p^2}{\omega^2},\qquad
\omega^2=\omega_p^2+c^2k^2.}
$$

For $\omega>\omega_p$, $k$ is real in this collisionless model and the wave propagates. Its [phase velocity](../../../../../phase-velocity.md) is $v_{\rm ph}=c/n>c$, while its [group velocity](../../../../../group-velocity.md) is $v_g=cn<c$; their product is $c^2$. A phase crest exceeding $c$ does not imply superluminal information transport. For $\omega<\omega_p$, the refractive-index square is negative and

$$
k=i\frac{\sqrt{\omega_p^2-\omega^2}}c,
\qquad \delta=\frac c{\sqrt{\omega_p^2-\omega^2}}.
$$

The transmitted field is evanescent rather than a traveling bulk wave. A sufficiently thick collisionless [plasma](../../../../../plasma-physics.md) reflects such radiation without Ohmic absorption. Collisions make the response complex and permit absorption. This accounts for a [plasma](../../../../../plasma-physics.md) cutoff and, qualitatively, the reflection of some radio frequencies by ionized atmospheric layers. The simple model describes transverse waves; [plasmas](../../../../../plasma-physics.md) also support longitudinal collective modes.

In a [metal](../../../../../metal.md), positive [ions](../../../../../ion.md) usually form a [crystal](../../../../../crystal.md) lattice. Mobile conduction [electrons](../../../../../electron.md) occupy states described by the [electronic band structure](../../../../../electronic-band-structure.md) and normally form a degenerate [Fermi gas](../../../../../fermi-gas.md). The conduction-electron [density](../../../../../density.md) is usually much higher than in a dilute gas [plasma](../../../../../plasma-physics.md). Thus its [plasma frequency](../../../../../plasma-frequency.md) is commonly in the optical or [ultraviolet](../../../../../ultraviolet.md) range, rather than the lower radio-frequency values possible in dilute [plasmas](../../../../../plasma-physics.md). [Electron](../../../../../electron.md) scattering from the lattice, defects and other excitations gives a finite relaxation rate. The distinction is not that every [plasma](../../../../../plasma-physics.md) is collisionless and every [metal](../../../../../metal.md) collisional: the controlling ratio for either material is $\omega/\nu$, together with its carrier [density](../../../../../density.md) and bound-charge response.

At sufficiently low frequency, $\omega\ll\nu$, the [metal](../../../../../metal.md)'s conductivity is approximately real, $\sigma_0=n_ee^2/(m\nu)$. In a good conductor the conduction current dominates the displacement current, $\sigma_0\gg\omega\epsilon_b$. The wave equation then gives

$$
k^2\simeq i\mu\sigma_0\omega,\qquad
\boxed{k\simeq(1+i)\sqrt{\frac{\mu\sigma_0\omega}{2}}=\frac{1+i}{\delta},
\quad\delta=\sqrt{\frac{2}{\mu\sigma_0\omega}}.}
$$

For example, a tangential electric field varies as

$$
E(z,t)=E_0e^{-z/\delta}\cos\left(\frac z\delta-\omega t\right).
$$

The current $\mathbf J=\sigma_0\mathbf E$ is therefore concentrated within a few skin depths of the surface: this is the [skin effect](../../../../../skin-effect.md). As frequency increases within this regime, $\delta\propto\omega^{-1/2}$. In a wire whose radius greatly exceeds $\delta$, only a thin outer region carries appreciable alternating current, increasing the effective resistance. In a conducting shield, the same penetration suppresses the field transmitted through a sufficiently thick wall.

The [Poynting theorem](../../../../../poynting-theorem.md) identifies the loss as [Joule heating](../../../../../joule-heating.md). The cycle-averaged heating [density](../../../../../density.md) for a complex conductivity is

$$
\langle\mathbf J\cdot\mathbf E\rangle=\frac12\operatorname{Re}\sigma\,|\mathbf E|^2.
$$

The [wave impedance](../../../../../wave-impedance.md) is $Z=\mu\omega/k$. For incidence from vacuum at normal incidence, the electric reflection amplitude is $r=(Z-Z_0)/(Z+Z_0)$, where $Z_0=\sqrt{\mu_0/\epsilon_0}$. A good conductor has small $|Z|$ and therefore strong reflection, while the part of the incident power entering it is dissipated over the [skin depth](../../../../../skin-depth.md).

At high enough frequency that $\omega\gg\nu$, a [metal](../../../../../metal.md)'s free-electron response also approaches the collisionless [plasma](../../../../../plasma-physics.md) form. The low-frequency formula $\delta\propto\omega^{-1/2}$ must not simply be extrapolated into that regime. Real optical behavior additionally depends on the [electronic band structure](../../../../../electronic-band-structure.md) and transitions between bands. Both [plasmas](../../../../../plasma-physics.md) and [metals](../../../../../metal.md) are therefore described by the same electromagnetic response framework, but their relevant densities, scattering rates and frequency regimes differ.

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

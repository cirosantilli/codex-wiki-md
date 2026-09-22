# Gravity-capillary wave

↑ **Parent:** [Capillary wave](capillary-wave.md)

A [gravity-capillary wave](gravity-capillary-wave.md) has restoring contributions from both [gravity](gravity.md) and [surface tension](surface-tension-split.md). Consider an initially resting, horizontally unbounded [liquid](liquid.md) layer of constant depth $h$, with uniform [mass density](density.md) $\rho$, [incompressible flow](incompressible-flow.md), [inviscid flow](inviscid-flow.md) and [irrotational flow](irrotational-flow.md). The upper [gas](gas.md) exerts constant [pressure](pressure-split.md) and has negligible inertia. Assume a clean interface with constant [surface tension](surface-tension-split.md) $\gamma$: no [surfactant](surfactant.md) stresses, imposed current or wind. The [wave amplitude](wave-amplitude.md) $a$ must satisfy $ka\ll1$ and $a\ll h$, so [linearized boundary conditions](linearized-boundary-condition.md) apply. Deep water means $kh\gg1$, rather than a particular depth in metres. [Brenner, Peacock, Stocker, Reis and Dunkel, MIT Nonlinear Dynamics II, §23.1, pp. 105–106](https://www.ocw.mit.edu/courses/18-354j-nonlinear-dynamics-ii-continuum-systems-spring-2015/6163837c5efa5d6ed969e535ec8f890c_MIT18_354JS15_lectureNotes.pdf)

Let $z=0$ be the undisturbed [free surface](free-surface.md), with [liquid](liquid.md) below it. [Potential flow](potential-flow.md) gives a [velocity potential](velocity-potential.md) $\phi$ with $\mathbf u=\nabla\phi$, and [incompressible flow](incompressible-flow.md) gives the [Laplace equation](laplace-equation.md). The linearized [kinematic boundary condition for a free-surface graph](kinematic-boundary-condition-for-a-free-surface-graph.md) and the [Unsteady Bernoulli equation](unsteady-bernoulli-equation.md), including [gravity](gravity.md) and the [Young–Laplace equation](young-laplace-equation.md), give

$$
\phi_{xx}+\phi_{zz}=0\quad(z<0),
\qquad
\eta_t=\phi_z,
\qquad
\phi_t+g\eta-\frac{\gamma}{\rho}\eta_{xx}=0\quad(z=0).
$$

Here $\eta(x,t)$ is the interface displacement; the signed small-slope [pressure](pressure-split.md) jump is $p_{\mathrm{liquid}}-p_{\mathrm{gas}}=-\gamma\eta_{xx}$. A [wave crest](wave-crest.md) has $\eta_{xx}<0$, so its [capillary pressure](capillary-pressure.md) is positive. Choose a right-travelling [Fourier mode](fourier-mode.md) of positive [wavenumber](wavenumber.md) $k$ and [angular frequency](angular-frequency.md) $\omega$:

$$
\eta=a\cos(kx-\omega t),
\qquad
\phi=\frac{a\omega}{k}e^{kz}\sin(kx-\omega t).
$$

The factor $e^{kz}$ decays into the deep [liquid](liquid.md), satisfies the [Laplace equation](laplace-equation.md), and makes $\phi_z=\eta_t$ at $z=0$. Substituting in the dynamic [boundary condition](boundary-condition.md) leaves

$$
-\frac{a\omega^2}{k}+ga+\frac{\gamma}{\rho}k^2a=0,
\qquad
\boxed{\omega^2=gk+\frac{\gamma}{\rho}k^3}.
$$

This derivation displays the two restoring contributions with the same sign. [Dimensional analysis](dimensional-analysis.md) also checks the result: $\gamma/\rho$ has units $\mathrm{m^3\,s^{-2}}$, so both $gk$ and $(\gamma/\rho)k^3$ have units $\mathrm{s^{-2}}$. [MIT Nonlinear Dynamics II, §23.1, equations (547)–(551): boundary conditions and dispersion](https://www.ocw.mit.edu/courses/18-354j-nonlinear-dynamics-ii-continuum-systems-spring-2015/6163837c5efa5d6ed969e535ec8f890c_MIT18_354JS15_lectureNotes.pdf)

At finite depth, a flat impermeable bottom at $z=-h$ requires $\phi_z=0$. Replacing $e^{kz}$ by the normalized vertical factor $\cosh(k(z+h))/\cosh(kh)$ makes the surface ratio $\phi_z/\phi=k\tanh(kh)$. Eliminating the mode amplitudes then gives

$$
\omega^2=\left(gk+\frac{\gamma}{\rho}k^3\right)\tanh(kh).
$$

Thus the same model supplies its own depth check: use the deep-water formula only when $\tanh(kh)$ is sufficiently close to one for the required accuracy. For example, $kh=3$ reduces $\omega$ by about $0.248\%$ relative to deep water, while $kh=1$ reduces it by about $12.7\%$. These percentages are calculations from this factor. [John W. M. Bush, Interfacial Phenomena, chapter 19, equation (19.4)](https://ocw.mit.edu/courses/18-357-interfacial-phenomena-fall-2010/04759cfc15c79928ca9f72a18b3864dd_MIT18_357F10_lec_all.pdf)

In deep water the [phase velocity](phase-velocity.md) magnitude follows a [wave crest](wave-crest.md), while the [group velocity](group-velocity.md) magnitude follows the [wave envelope](envelope-waves.md) of a narrow [wave packet](wave-packet.md). Differentiating the positive-frequency [dispersion relation](dispersion-relation-split.md) gives

$$
c_p=\frac{\omega}{k}=\sqrt{\frac{g}{k}+\frac{\gamma k}{\rho}},
\qquad
c_g=\frac{d\omega}{dk}
=\frac{g+3\gamma k^2/\rho}{2\sqrt{gk+\gamma k^3/\rho}},
\qquad
\frac{c_g}{c_p}=\frac{1+3(k\ell_c)^2}{2\left(1+(k\ell_c)^2\right)}.
$$

For $k\ell_c\ll1$, the [surface gravity wave](surface-gravity-wave.md) limit has $c_g\simeq c_p/2$. For $k\ell_c\gg1$, the [deep-water capillary-wave dispersion relation](deep-water-capillary-wave-dispersion-relation.md) has $c_g\simeq3c_p/2$: a [wave crest](wave-crest.md) slips backward relative to the faster [wave envelope](envelope-waves.md), even while both advance. Neither speed is the oscillating [fluid element](fluid-element.md)'s own [velocity](velocity.md). [John W. M. Bush, Interfacial Phenomena, chapter 19, equation (19.5) and the two group-speed limits](https://ocw.mit.edu/courses/18-357-interfacial-phenomena-fall-2010/04759cfc15c79928ca9f72a18b3864dd_MIT18_357F10_lec_all.pdf)

There is a particularly neat coincidence at the crossover. Differentiate $c_p^2=g/k+\gamma k/\rho$: its unique minimum is at $k_c=\sqrt{\rho g/\gamma}=1/\ell_c$, exactly where the restoring terms are equal. Therefore

$$
c_{p,\min}=\left(\frac{4g\gamma}{\rho}\right)^{1/4},
\qquad c_g(k_c)=c_p(k_c).
$$

For the stipulated parameters in [capillary length](capillary-length.md), the minimum is $0.231\,\mathrm{m\,s^{-1}}$. At $\lambda=3\,\mathrm{mm}$, direct substitution gives $f=\omega/(2\pi)\simeq131\,\mathrm{Hz}$, $c_p\simeq0.394\,\mathrm{m\,s^{-1}}$ and $c_g\simeq0.580\,\mathrm{m\,s^{-1}}$. This short [wavelength](wavelength.md) is capillary dominated, but its [group velocity](group-velocity.md) is still slightly below the pure-capillary ratio $3c_p/2$ because [gravity](gravity.md) has not vanished.

**Table of contents**

- [Minimum phase speed of a gravity-capillary wave](minimum-phase-speed-of-a-gravity-capillary-wave.md)

## ↑ Ancestors (6)

1. [Capillary wave](capillary-wave.md)
2. [Surface tension](surface-tension-split.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Capillary length](capillary-length.md)
- [Capillary wave](capillary-wave.md)
- [Dispersion relation](dispersion-relation-split.md)
- [Elastic-cover frequency ratio for water waves](elastic-cover-frequency-ratio-for-water-waves.md)
- [Gravity-capillary wave](gravity-capillary-wave.md)
- [Minimum phase speed of a gravity-capillary wave](minimum-phase-speed-of-a-gravity-capillary-wave.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019/section-a/3/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2021/section-a/3/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2/section-b/b7/solution.md)

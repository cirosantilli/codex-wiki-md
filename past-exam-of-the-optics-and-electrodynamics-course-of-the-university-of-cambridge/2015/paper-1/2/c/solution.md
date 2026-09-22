<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Both [Thomson scattering](../../../../../thomson-scattering.md) and [Rayleigh scattering](../../../../../rayleigh-scattering.md) can be understood as radiation from a dipole driven by the incident [electric field](../../../../../electric-field-split.md). Their different [frequency](../../../../../frequency.md) dependences come from the response of a free charge compared with a [bound charge](../../../../../bound-charge.md).

For a free particle of charge $q$ and [mass](../../../../../mass.md) $m$, a harmonic field gives $m\ddot{\mathbf x}=q\mathbf E$, hence $\mathbf p=q\mathbf x=-q^2\mathbf E/(m\omega^2)$. The radiated field contains two time derivatives of $\mathbf p$, cancelling the response's $\omega^{-2}$. The Thomson cross section is consequently independent of [frequency](../../../../../frequency.md) in the classical low-recoil regime:

$$
r_q=\frac{q^2}{4\pi\epsilon_0mc^2},\qquad
\boxed{\sigma_T=\frac{8\pi}{3}r_q^2}.
$$

For incident [linear polarization](../../../../../linear-polarization.md) with unit polarization $\boldsymbol\epsilon$, summing over outgoing polarizations gives $d\sigma/d\Omega=r_q^2[1-|\widehat{\mathbf n}\cdot\boldsymbol\epsilon|^2]$. Radiation vanishes along the acceleration and is strongest perpendicular to it. Averaging an incident [unpolarized light](../../../../../unpolarized-light.md) beam gives

$$
\frac{d\sigma_T}{d\Omega}=\frac{r_q^2}{2}(1+\cos^2\Theta),
$$

where $\Theta$ is the [scattering angle](../../../../../scattering-angle.md). Scattering through $90^\circ$ is fully linearly polarized perpendicular to the [scattering plane](../../../../../scattering-plane.md) for this ideal isotropic dipole model. The [electron](../../../../../electron.md) case dominates over equally charged heavier particles because the cross section scales as $m^{-2}$. [recoil](../../../../../recoil.md) corrections become necessary when [photon energy](../../../../../photon-energy.md) is no longer small compared with $mc^2$.

For a [bound charge](../../../../../bound-charge.md) with [natural frequency](../../../../../natural-frequency.md) $\omega_0$ and damping rate $\gamma_d$,

$$
\mathbf p=\alpha_{\rm e}(\omega)\mathbf E,\qquad
\alpha_{\rm e}=\frac{q^2/m}{\omega_0^2-\omega^2-i\gamma_d\omega}.
$$

Far below [resonance](../../../../../resonance.md), $\alpha_{\rm e}$ is approximately constant, so

$$
\boxed{\sigma_R=\frac{k^4|\alpha_{\rm e}|^2}{6\pi\epsilon_0^2}
\ \propto\omega^4\propto\lambda^{-4}}.
$$

This is [Rayleigh scattering](../../../../../rayleigh-scattering.md). It requires a scatterer small compared with the [wavelength](../../../../../wavelength.md) and, for the simple expression, an isotropic linear dipole response. Atoms, molecules and small [dielectric](../../../../../dielectric.md) particles provide examples. The stronger scattering of shorter visible [wavelengths](../../../../../wavelength.md) explains blue skylight; [absorption](../../../../../absorption-electromagnetic-radiation.md) and the nonuniform solar spectrum prevent treating that simple scaling as a complete color calculation.[section 9.6, bound-charge response and low-frequency limit](../../../../../rayleigh-scattering-by-richard-fitzpatrick.md)

For isotropic electric scatterers the normalized angular and polarization patterns are the same as in [Thomson scattering](../../../../../thomson-scattering.md). The [frequency](../../../../../frequency.md) scaling distinguishes their limits: a free charge has a displacement proportional to $\omega^{-2}$, whereas a tightly [bound charge](../../../../../bound-charge.md) has an approximately frequency-independent displacement. Near [resonance](../../../../../resonance.md), far outside the small-particle limit, or with anisotropic [polarizability](../../../../../electric-polarizability.md), the simple Rayleigh formula must be modified. In particular, the electric-only pattern must not silently be applied to a perfectly conducting sphere whose magnetic dipole response is also retained.

A scattering measurement should subtract stray-light and detector backgrounds, control scatterer density and optical thickness, and calibrate detector response and incident [power](../../../../../power.md) when comparing [wavelengths](../../../../../wavelength.md). A polarization analyzer at $90^\circ$ tests the dipole pattern; multiple scattering or unresolved nonisotropic contributions can reduce its polarization.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

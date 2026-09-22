<h1 id="section-d/d9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To determine a [crystal structure](../../../../../../crystal-structure.md), scatter probes whose [wavelength](../../../../../../wavelength.md) is comparable to atomic spacings, typically $0.1\,\mathrm{nm}$. [X-ray diffraction](../../../../../../x-ray-diffraction.md), [neutron diffraction](../../../../../../neutron-diffraction.md) and [electron diffraction](../../../../../../electron-diffraction.md) probe periodic order through coherent elastic scattering. With incident and outgoing [wavevectors](../../../../../../wavevector.md) $\mathbf k_i,\mathbf k_f$, define $\mathbf Q=\mathbf k_i-\mathbf k_f$. Elastic scattering has $|\mathbf k_i|=|\mathbf k_f|$ and constructive [interference](../../../../../../interference-wave-propagation.md) occurs when $\mathbf Q=\mathbf G$, a [reciprocal lattice](../../../../../../reciprocal-lattice.md) vector. The equivalent [Bragg's law](../../../../../../bragg-s-law.md) is

$$
\boxed{2d_{hkl}\sin\theta=n\lambda,}
$$

where the detector scattering angle is $2\theta$, not $\theta$. Peak positions reveal plane spacings and the [unit cell](../../../../../../unit-cell.md); systematic absent reflections constrain centring and the atomic basis.

For [X-ray diffraction](../../../../../../x-ray-diffraction.md), a laboratory tube or a [synchrotron](../../../../../../synchrotron.md) supplies a collimated beam. In a monochromatic single-crystal experiment a [goniometer](../../../../../../goniometer.md) rotates the specimen and an area detector records reflection positions and integrated [wave intensities](../../../../../../intensity-physics.md). A powder experiment uses many randomly oriented crystallites; the reflections form cones recorded as rings or peaks versus $2\theta$, permitting indexing and determination of lattice constants without selecting one crystallite. For a cubic cell, for example, $d_{hkl}=a/\sqrt{h^2+k^2+l^2}$. The white-beam [Laue method](../../../../../../laue-method.md) is especially useful for [crystal](../../../../../../crystal.md) orientation.

The [crystal basis structure factor](../../../../../../crystal-basis-structure-factor.md) is

$$
F_{\mathbf G}=\sum_j f_j(\mathbf Q)e^{i\mathbf G\cdot\mathbf r_j},\qquad I_{\mathbf G}\propto|F_{\mathbf G}|^2
$$

after geometric and thermal corrections, including the [Debye–Waller factor](../../../../../../debye-waller-factor.md). For [X-rays](../../../../../../x-ray.md), $f_j$ describes scattering from the atomic [electron density](../../../../../../electron-density.md). Thus positions provide lattice geometry while relative [wave intensities](../../../../../../intensity-physics.md) constrain atomic positions and species. [Wave intensities](../../../../../../intensity-physics.md) do not directly give the [phases](../../../../../../phase-waves.md) of $F_{\mathbf G}$: structure refinement or other constraints must address the [phase problem](../../../../../../phase-problem.md).

[Neutron diffraction](../../../../../../neutron-diffraction.md) uses a reactor or spallation source, wavelength selection and a detector bank or time-of-flight detection. Neutrons interact with nuclei through nuclear scattering lengths that vary between elements and isotopes rather than simply with atomic number. This makes them useful for light atoms, isotope contrast and distinguishing some neighbours in the periodic table; their magnetic interaction also probes magnetic order. [Electron diffraction](../../../../../../electron-diffraction.md) in a transmission electron microscope gives strong signals from very small thin crystallites, although strong multiple scattering often complicates quantitative [wave intensity](../../../../../../intensity-physics.md) analysis. These techniques complement one another.

A [phonon dispersion relation](../../../../../../phonon-dispersion-relation.md) requires both momentum and [energy](../../../../../../energy-split.md) transfer, so elastic [diffraction](../../../../../../diffraction.md) alone is insufficient. In coherent [inelastic neutron scattering](../../../../../../inelastic-neutron-scattering.md), the measured transfers for phonon creation are

$$
\boxed{\hbar\mathbf Q=\hbar(\mathbf k_i-\mathbf k_f),\quad
\hbar\omega=E_i-E_f,\quad
\mathbf Q=\mathbf G+\mathbf q,\quad\omega=\omega_s(\mathbf q).}
$$

Here $\mathbf q$ is the [phonon](../../../../../../phonon.md) [wavevector](../../../../../../wavevector.md) reduced into a [Brillouin zone](../../../../../../brillouin-zone.md), and $s$ labels an [acoustic phonon branch](../../../../../../acoustic-phonon-branch.md) or [optical phonon branch](../../../../../../optical-phonon-branch.md). Negative [energy](../../../../../../energy-split.md) transfer corresponds to annihilating an already occupied [phonon](../../../../../../phonon.md). For neutrons $E=\hbar^2k^2/(2m_n)$, so wavelength and [energy](../../../../../../energy-split.md) selection are linked. Typical thermal-neutron energies of a few to tens of millielectronvolts ($1\,\mathrm{meV}=10^{-3}$ [electronvolts](../../../../../../electronvolt.md)) are well matched to many lattice vibrations.

A [triple-axis spectrometer](../../../../../../triple-axis-spectrometer.md) uses a [monochromator](../../../../../../monochromator.md) crystal to select $\mathbf k_i$, the sample as the second scattering axis, and an analyser crystal to select $\mathbf k_f$ before detection. Rotate these elements and the specimen to hold $\mathbf Q$ fixed while scanning $E_i-E_f$; inelastic peaks locate $\omega_s(\mathbf q)$. Repeat at different $\mathbf q$ along symmetry directions to map the [phonon dispersion relation](../../../../../../phonon-dispersion-relation.md). The [dynamic structure factor](../../../../../../dynamic-structure-factor.md) governs peak weights, including the selection of [phonon](../../../../../../phonon.md) polarization by the scattering geometry. A time-of-flight spectrometer instead infers outgoing neutron [energy](../../../../../../energy-split.md) from travel time over a known flight path and records many directions simultaneously.

[Inelastic X-ray scattering](../../../../../../inelastic-x-ray-scattering.md) can also resolve [phonons](../../../../../../phonon.md) when very high [energy resolution](../../../../../../energy-resolution.md) is available. Optical [Raman scattering](../../../../../../raman-scattering.md) and [Brillouin scattering](../../../../../../brillouin-scattering.md) measure vibrations near the zone centre because photon momentum transfers are small compared with a typical [reciprocal lattice](../../../../../../reciprocal-lattice.md) spacing; they complement, rather than generally map the entire zone like, momentum-resolved neutron measurements. [Ultrasound](../../../../../../ultrasound.md) measurements give the long-wavelength [sound speed](../../../../../../speed-of-sound.md), the initial slope $d\omega/dq$ of an [acoustic phonon branch](../../../../../../acoustic-phonon-branch.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D9](../../d9.md)
3. [Section D](../../../section-d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

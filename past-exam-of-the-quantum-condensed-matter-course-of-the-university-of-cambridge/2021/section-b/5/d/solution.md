<h1 id="section-b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For one conduction electron per atom, let $n_a$ be the atom density. [State counting in a Bloch band](../../../../../state-counting-in-a-bloch-band.md) gives the [Fermi wavevector](../../../../../fermi-wavevector.md) $k_F=(3\pi^2n_a)^{1/3}$. The [Debye model](../../../../../debye-model.md) preserves the three vibrational modes per atom by a spherical [Debye wavevector](../../../../../debye-wavevector.md) cutoff $q_D=(6\pi^2n_a)^{1/3}$, so

$$
\boxed{q_D=2^{1/3}k_F\simeq1.26k_F.}
$$

Both wavevectors are of order the inverse atomic spacing. The numerical factor uses the spherical Debye approximation; a real zone boundary and the largest-frequency mode depend on direction and branch. Because $q_D<2k_F$, short-wavelength acoustic [phonons](../../../../../phonon.md) can scatter [Fermi surface](../../../../../fermi-surface.md) electrons through substantial angles. For nearly elastic scattering within a spherical Fermi surface,

$$
q=2k_F\sin(\theta/2),\qquad1-\cos\theta=\frac{q^2}{2k_F^2}.
$$

Near room temperature, when a substantial fraction of the phonon spectrum is occupied, [electron-phonon scattering](../../../../../electron-phonon-scattering.md) is often the main source of [electrical resistance](../../../../../electrical-resistance.md). For $T\gg\Theta_D$, the phonon population and scattering rate are approximately proportional to $T$, giving $\rho\propto T$, $\sigma\propto T^{-1}$ and roughly constant $K_e$ when the [Wiedemann-Franz law](../../../../../wiedemann-franz-law.md) holds.

For [small-angle electron-phonon transport at low temperature](../../../../../small-angle-electron-phonon-transport-at-low-temperature.md), thermally active acoustic modes instead have

$$
q_T\sim\frac{k_BT}{\hbar c_s}=q_D\frac{T}{\Theta_D}\ll k_F.
$$

They predominantly scatter forward. The factor $1-\cos\theta$ makes such collisions inefficient at relaxing an electrical current, while a phonon energy of order $k_BT$ can still substantially change an electron's thermal excitation. Heat-current relaxation therefore need not share the charge-current relaxation time. In the clean three-dimensional acoustic-phonon model this gives $\tau_Q^{-1}\propto T^3$ but $\tau_\sigma^{-1}\propto T^5$, so the phonon-limited electrical resistivity scales as $T^5$ and $K_e\propto T^{-2}$. These laws describe the regime before residual elastic scattering takes over; at sufficiently low temperature impurities give nearly constant residual resistivity and $K_e\propto T$, restoring the usual [Lorenz number](../../../../../lorenz-number.md).[Electron-phonon scattering: distinct low-temperature thermal and electrical transport relaxation rates](https://home.itp.ac.ru/~grigorev/LectureSlides/MetalsLecture2.pdf)

[Phonons](../../../../../phonon.md) also transport heat themselves, with $K_{\rm ph}\simeq c_{\rm ph}c_s\ell_{\rm ph}/3$. At low temperature their population decreases and their [phonon mean free path](../../../../../phonon-mean-free-path.md) can become boundary- or defect-limited. At higher temperature [Umklapp scattering](../../../../../umklapp-scattering.md) can relax the phonon heat current. Such lattice conduction is an additional contribution, not the quantity constrained by the electronic [Wiedemann-Franz law](../../../../../wiedemann-franz-law.md).

## ↑ Ancestors (14)

1. [D](../d.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Debye model](../../../../debye-model.md) treats a three-dimensional solid as an isotropic elastic continuum with three independent acoustic [phonon polarizations](../../../../phonon-polarization.md). It assumes harmonic [normal modes](../../../../normal-mode.md), a linear [dispersion relation](../../../../dispersion-relation-split.md) $\omega=vq$, and equilibrium [Bose-Einstein statistics](../../../../bose-einstein-statistics.md) with zero [phonon](../../../../phonon.md) [chemical potential](../../../../chemical-potential-split.md). Real anisotropy and nonlinear dispersion are replaced by one effective [Debye sound speed](../../../../debye-sound-speed.md). A cutoff restores the finite number of atomic vibrational degrees of freedom; the continuum itself would otherwise have infinitely many modes.

For sample [volume](../../../../volume.md) $V$, the [wavevector](../../../../wavevector.md) state density is $V/(2\pi)^3$ per polarization. Counting a sphere gives

$$
\mathcal N(q)=3\frac{V}{(2\pi)^3}\frac{4\pi q^3}{3}
=\frac{Vq^3}{2\pi^2}.
$$

There are $3N$ modes for $N$ atoms. Hence

$$
q_D^3=6\pi^2\frac NV,
\qquad\boxed{\omega_D=v\left(6\pi^2n_a\right)^{1/3},\quad n_a=N/V.}
$$

The associated [phonon density of states](../../../../phonon-density-of-states.md) is

$$
g(\omega)=\frac{3V\omega^2}{2\pi^2v^3}
=\frac{9N\omega^2}{\omega_D^3},\qquad0<\omega<\omega_D.
$$

If longitudinal and transverse [sound speeds](../../../../speed-of-sound.md) differ, use $3/v^3=1/v_L^3+2/v_T^3$ for the low-frequency count. The [Debye frequency](../../../../debye-frequency.md) is an effective mode-counting cutoff, not a claim that every actual branch terminates at exactly that frequency.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

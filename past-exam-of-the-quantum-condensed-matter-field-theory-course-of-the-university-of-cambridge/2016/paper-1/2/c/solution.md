<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [contact-interaction Bose-gas field integral](../../../../../contact-interaction-bose-gas-field-integral.md) for a homogeneous three-dimensional [weakly interacting Bose gas](../../../../../weakly-interacting-bose-gas.md) with repulsive short-range interaction as the standard model. Let particle mass be $m_b$, [scattering length](../../../../../scattering-length-from-a-partial-wave-s-matrix.md) $a_s>0$, physical coupling $g=4\pi\hbar^2a_s/m_b$ and gas parameter $na_s^3\ll1$. These are symbolic model definitions, not supplied numerical parameters. The grand-canonical coherent-state integral has periodic fields and action

$$
S_E=\int_0^{\beta\hbar}d\tau\int d^3x\left[\bar\psi\left(\hbar\partial_\tau-\frac{\hbar^2\nabla^2}{2m_b}-\mu\right)\psi+\frac g2(\bar\psi\psi)^2\right].
$$

The contact term is the normal symbol of $g\hat\psi^{\dagger2}\hat\psi^2/2$. In three dimensions a [contact interaction](../../../../../contact-interaction-quantum-mechanics.md) needs a regulator and coupling matched to the measured [scattering length](../../../../../scattering-length-from-a-partial-wave-s-matrix.md); the displayed $g$ is the low-energy physical coupling. This field integral is useful because an ordered saddle and its quantum/thermal fluctuations follow from the same action.

Stationarity with respect to $\bar\psi$ gives the imaginary-time [Gross–Pitaevskii equation](../../../../../gross-pitaevskii-equation.md). A uniform saddle exists at $\mu>0$ with $\psi_0=\sqrt{n_0}e^{i\theta_0}$ and [condensate density](../../../../../condensate-density.md) $n_0=\mu/g$. Its arbitrary phase reflects global $U(1)$ [symmetry](../../../../../symmetry-physics.md); a selected condensate fixes a phase in the thermodynamic symmetry-breaking description. Write $\psi=\sqrt{n_0}+\eta$ after choosing that phase. Linear terms vanish, and the quadratic part is

$$
S_2=\int d\tau\,d^3x\left[\bar\eta\left(\hbar\partial_\tau-\frac{\hbar^2\nabla^2}{2m_b}+\mu\right)\eta+\frac\mu2(\eta^2+\bar\eta^2)\right].
$$

With $\varepsilon_k=\hbar^2k^2/(2m_b)$ and the Fourier convention $e^{i\mathbf k\cdot\mathbf x-i\omega_n\tau}$, the paired quadratic kernel is

$$
\mathcal M(\mathbf k,\omega_n)=\begin{pmatrix}-i\hbar\omega_n+\varepsilon_k+\mu&\mu\\\mu&i\hbar\omega_n+\varepsilon_k+\mu\end{pmatrix},\qquad \det\mathcal M=(\hbar\omega_n)^2+\varepsilon_k(\varepsilon_k+2\mu).
$$

The one-half in the [Nambu spinor](../../../../../nambu-spinor.md) action removes pair double counting. Analytic continuation of the inverse kernel gives **the Bogoliubov dispersion**

$$
\boxed{E_k=\sqrt{\varepsilon_k(\varepsilon_k+2gn_0)},\qquad E_k\simeq\hbar c_s k,\qquad c_s=\sqrt{gn_0/m_b}.}
$$

At high [momentum](../../../../../momentum-split.md) it approaches the free-particle [kinetic energy](../../../../../kinetic-energy.md) plus its mean-field shift. The crossover scale is the [healing length](../../../../../healing-length.md) $\xi=\hbar/\sqrt{2m_bgn_0}$. Gaussian integration adds a fluctuation [determinant](../../../../../determinant.md) to the saddle [free energy](../../../../../thermodynamic-free-energy.md). Expressed using the physical three-dimensional coupling, its zero-temperature integrand can be regularized as $\tfrac12[E_k-\varepsilon_k-\mu+\mu^2/(2\varepsilon_k)]$; the subtraction follows from [renormalization of a three-dimensional dilute-gas contact coupling](../../../../../renormalization-of-a-three-dimensional-dilute-gas-contact-coupling.md), not discarding an infinite answer arbitrarily. The thermal contribution is $k_BT\int d^3k/(2\pi)^3\log(1-e^{-\beta E_k})$. A calculation beyond mean field must keep that matching and its thermodynamic derivatives consistent.

The [density-phase action of a Bose gas](../../../../../density-phase-action-of-a-bose-gas.md) makes the physical content clear, $\psi=\sqrt{n_0+\delta n}\,e^{i\theta}$. Up to a periodic density total derivative, the long-wavelength quadratic action contains

$$
S_2=\int d\tau\,d^3x\left[i\hbar\delta n\,\partial_\tau\theta+\frac g2(\delta n)^2+\frac{\hbar^2n_0}{2m_b}(\nabla\theta)^2+\frac{\hbar^2}{8m_bn_0}(\nabla\delta n)^2\right].
$$

[number-phase conjugacy](../../../../../number-phase-conjugacy.md) pairs the density fluctuation and phase in the [quadratic density-phase action](../../../../../quadratic-density-phase-action.md). Dropping the density-gradient term only in the long-wave limit and completing the density Gaussian square gives the [Bose-gas phase-only action](../../../../../bose-gas-phase-only-action.md)

$$
S_{\theta}=\frac12\int d\tau\,d^3x\left[\frac{\hbar^2}{g}(\partial_\tau\theta)^2+\frac{\hbar^2n_0}{m_b}(\nabla\theta)^2\right].
$$

This has the same sound pole. A term $i\hbar n_0\partial_\tau\theta$ is also present before restricting to the smooth zero-winding sector; although locally a total derivative, it cannot in general be ignored in topologically nontrivial sectors. The density and phase variables describe the same coupled Bogoliubov branch, not a second independent massive particle simply because the density has a static restoring cost.[§2.3, printed pp.29–38: superfluid phase stiffness, amplitude fluctuations and phase dynamics](../../../../../physics-215c-quantum-field-theory-part-3-by-john-mcgreevy.md)

A phase gradient carries superflow $\mathbf v_s=(\hbar/m_b)\nabla\theta$. Its energy cost defines the [superfluid number density](../../../../../superfluid-number-density.md). At leading mean-field order the stiffness uses $n_0$, but [condensate density](../../../../../condensate-density.md) and [superfluid number density](../../../../../superfluid-number-density.md) are different observables: for a Galilean-invariant continuum gas at zero [temperature](../../../../../temperature-split.md) the latter is the full density even when interactions deplete the condensate. Bogoliubov coefficients give $v_k^2=[(\varepsilon_k+gn_0)/E_k-1]/2$ and a small zero-temperature depletion of relative order $\sqrt{na_s^3}$ in three dimensions. Large depletion or strong long-wavelength phase fluctuations would invalidate the small-fluctuation saddle approximation.

The [Landau criterion](../../../../../landau-criterion.md) for creating excitations is $v_L=\inf_{k>0}E_k/(\hbar k)=c_s$ for this homogeneous dispersion. Thus **repulsion produces a linear sound mode and a positive critical velocity from the [Landau criterion](../../../../../landau-criterion.md)**, whereas an ideal quadratic gas has zero value of this criterion. Vortices, obstacles and nucleation can reduce an actual flow threshold below $c_s$; the criterion alone is not a complete theory of metastable flow. At finite [temperature](../../../../../temperature-split.md) thermal [quasiparticles](../../../../../quasiparticle.md) reduce the [superfluid number density](../../../../../superfluid-number-density.md). Dimensionality and finite size also matter: the uniform three-dimensional weak-depletion condensate expansion must not be transferred unchanged to a one- or two-dimensional thermodynamic system. The field integral provides systematic corrections only within its dilute, stable and sufficiently weak-fluctuation regime.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

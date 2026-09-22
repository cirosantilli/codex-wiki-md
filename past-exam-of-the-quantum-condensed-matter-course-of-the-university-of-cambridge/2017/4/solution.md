<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Noninteracting [spectral line](../../../spectral-line.md).** Treat $\mathbf k$ as a [wavevector](../../../wavevector.md), so physical [crystal momentum](../../../crystal-momentum.md) is $\hbar\mathbf k$. Write $\Omega_{\mathbf k}=\varepsilon_{\mathbf k}/\hbar$; an [energy](../../../energy-split.md) zero at the [chemical potential](../../../chemical-potential-split.md) can be chosen throughout. The temporal factor of a noninteracting state is $e^{-i\Omega_{\mathbf k}t}$. With the [Fourier transform](../../../fourier-transform-split.md) convention $\widetilde\psi(\omega)=\int dt\,e^{i\omega t}\psi(t)$,

$$
\widetilde\psi_{\mathbf k}(\omega)=2\pi\psi_{\mathbf k}(0)\delta(\omega-\Omega_{\mathbf k}).
$$

Thus its normalized [frequency](../../../frequency.md) [spectral function](../../../spectral-function.md) is

$$
\boxed{A_0(\mathbf k,\omega)=\delta(\omega-\Omega_{\mathbf k}).}
$$

One should not square the delta distribution as if it were an ordinary finite-time transition amplitude. More precisely, the fermionic [retarded Green function](../../../retarded-green-function.md) is $G_0^R(\mathbf k,t)=-i\Theta(t)e^{-i\Omega_{\mathbf k}t}$. Its [Fourier transform](../../../fourier-transform-split.md) is $(\omega-\Omega_{\mathbf k}+i0^+)^{-1}$, whose negative imaginary part divided by $\pi$ is the same delta peak.

**Interactions and lifetime.** Interactions change the dispersion through the real part of the [self-energy](../../../self-energy.md) and permit decay into other excitations through its imaginary part. In the simplest quasiparticle-pole model, [exponential decay](../../../exponential-decay.md) of the retarded amplitude gives

$$
G^R(\mathbf k,t)=-i\Theta(t)e^{-i\Omega_{\mathbf k}^*t-\Gamma_{\mathbf k}t},\qquad \Gamma_{\mathbf k}>0.
$$

Performing the causal integral,

$$
G^R(\mathbf k,\omega)=-i\int_0^\infty e^{[i(\omega-\Omega_{\mathbf k}^*)-\Gamma_{\mathbf k}]t}\,dt=\frac1{\omega-\Omega_{\mathbf k}^*+i\Gamma_{\mathbf k}}.
$$

The corresponding [Lorentzian quasiparticle spectral peak](../../../lorentzian-quasiparticle-spectral-peak.md) is

$$
\boxed{A(\mathbf k,\omega)=-\frac1\pi\operatorname{Im}G^R=\frac1\pi\frac{\Gamma_{\mathbf k}}{(\omega-\varepsilon_{\mathbf k}^*/\hbar)^2+\Gamma_{\mathbf k}^2}.}
$$

Its total [frequency](../../../frequency.md) integral is one. The exponential amplitude lifetime is $1/\Gamma_{\mathbf k}$; the probability lifetime is $1/(2\Gamma_{\mathbf k})$. Describing $\Gamma_{\mathbf k}$ as a scattering rate therefore requires the lifetime convention to be specified. The [energy](../../../energy-split.md) half-width is $\hbar\Gamma_{\mathbf k}$.

A general interacting [electron](../../../electron.md) is more accurately described by $G^R=Z_{\mathbf k}/(\omega-\Omega^*_{\mathbf k}+i\Gamma_{\mathbf k})+G^R_{\mathrm{inc}}$ near the pole. The coherent peak then integrates to the [quasiparticle residue](../../../quasiparticle-residue.md) $Z_{\mathbf k}$ and an incoherent continuum carries the remaining weight. In an energy-unit [self-energy](../../../self-energy.md) convention,

$$
G^R=\frac1{\omega-\varepsilon^0_{\mathbf k}/\hbar-\Sigma^R(\mathbf k,\omega)/\hbar},\qquad \varepsilon^*_{\mathbf k}=\varepsilon^0_{\mathbf k}+\operatorname{Re}\Sigma^R(\mathbf k,\varepsilon^*_{\mathbf k}/\hbar).
$$

Linearizing the real denominator gives $Z=[1-\hbar^{-1}\partial_\omega\operatorname{Re}\Sigma^R]^{-1}$ and $\Gamma=-Z\operatorname{Im}\Sigma^R/\hbar$ at the pole. The requested unit-weight Lorentzian is the normalized [quasiparticle](../../../quasiparticle.md) model, not the most general exact interacting spectrum.

**Peak position and width.** At fixed $\mathbf k$, put $\gamma=\gamma(\mathbf k)>0$ and $\Omega=\hbar k^2/(2m^*)$. Differentiation gives

$$
\frac{\partial A}{\partial\omega}=-\frac{2\gamma(\omega-\Omega)}{\pi[(\omega-\Omega)^2+\gamma^2]^2}.
$$

It is positive for $\omega<\Omega$ and negative for $\omega>\Omega$, so the only maximum is at $\Omega$, with height $1/(\pi\gamma)$. Setting $A$ to half this height gives $(\omega-\Omega)^2=\gamma^2$. Therefore

$$
\boxed{\omega_{\max}=\frac{\hbar k^2}{2m^*},\qquad \mathrm{HWHM}_\omega=\gamma(\mathbf k),\qquad \mathrm{FWHM}_\omega=2\gamma(\mathbf k).}
$$

In [energy](../../../energy-split.md) units the maximum is $\hbar^2k^2/(2m^*)$ and the half-width is $\hbar\gamma(\mathbf k)$. [Frequency](../../../frequency.md) dependence of the [self-energy](../../../self-energy.md) would require reconsidering both the shape and peak position.

**[Fermi gas](../../../fermi-gas.md) and [Fermi liquid](../../../fermi-liquid-split.md).** A noninteracting [Fermi gas](../../../fermi-gas.md) has a delta-function [spectral line](../../../spectral-line.md) at its bare dispersion for every [momentum](../../../momentum-split.md). A normal three-dimensional [Fermi liquid](../../../fermi-liquid-split.md) has a shifted coherent peak plus incoherent spectral weight; close to the [Fermi surface](../../../fermi-surface.md) its width scales as $(\varepsilon-\mu)^2+(\pi k_BT)^2$. At zero [temperature](../../../temperature-split.md) the peak becomes arbitrarily sharp at the [Fermi surface](../../../fermi-surface.md), while it broadens farther away. [Spectral functions](../../../spectral-function.md) include addition and removal weight; occupied-only photoemission contains an extra Fermi factor.

<a id="4/image-a-free-spectral-line-and-broadened-quasiparticle-peaks-with-a-separate-incoherent-background"></a>
![](../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2017-quasiparticle-spectra.png)

**[Figure 4](#4/image-a-free-spectral-line-and-broadened-quasiparticle-peaks-with-a-separate-incoherent-background). A free spectral line and broadened quasiparticle peaks, with a separate incoherent background**.

**Photoemission measurement.** A [photon](../../../photon.md) of known [energy](../../../energy-split.md) $h\nu$ ejects an [electron](../../../electron.md). Measure its [kinetic energy](../../../kinetic-energy.md) $E_{\mathrm{kin}}$ and emission direction. For [binding energy](../../../binding-energy.md) $E_B\geq0$ below the [Fermi level](../../../fermi-level.md) and the appropriate calibrated [work function](../../../work-function.md) $\Phi$, [conservation of energy](../../../conservation-of-energy.md) gives

$$
\boxed{E_{\mathrm{kin}}=h\nu-\Phi-E_B.}
$$

[Conservation of momentum](../../../momentum-conservation.md) parallel to a periodic surface gives

$$
\mathbf k_{i,\parallel}+\mathbf q_{\gamma,\parallel}=\mathbf k_{\mathrm{out},\parallel}+\mathbf G_\parallel,\qquad k_{\mathrm{out},\parallel}=\frac{\sqrt{2m_0E_{\mathrm{kin}}}}{\hbar}\sin\theta,
$$

where $\mathbf G_\parallel$ is a surface reciprocal-lattice vector. At suitable [photon](../../../photon.md) energies the [photon](../../../photon.md) [momentum](../../../momentum-split.md) can be neglected; at higher energies it must be retained. The surface breaks perpendicular translation symmetry, so the perpendicular [crystal momentum](../../../crystal-momentum.md) generally needs a final-state model. A two-dimensional band can be reconstructed directly from the parallel components.

Within the [sudden approximation](../../../sudden-approximation.md) and [electric-dipole approximation](../../../electric-dipole-approximation.md), [photoemission intensity and spectral function](../../../photoemission-intensity-and-spectral-function.md) are related by

$$
I(\mathbf k,E)\propto|\mathcal M(\mathbf k,h\nu,\text{polarization})|^2 f(E)A_E(\mathbf k,E),\qquad A_E(\mathbf k,E)=\frac1\hbar A(\mathbf k,E/\hbar).
$$

Here $E$ is measured relative to the [chemical potential](../../../chemical-potential-split.md). Instrumental resolution convolves the product and inelastic scattering adds background. Thus [ARPES](../../../angle-resolved-photoemission-spectroscopy.md) maps the occupied [electron removal spectral function](../../../electron-removal-spectral-function.md), weighted by a [matrix element](../../../matrix-element.md); it does not measure the full unoccupied spectrum or an unweighted [spectral function](../../../spectral-function.md) automatically. Bright ridges give dispersions, and intrinsic widths give decay information after instrumental effects are removed.

**Reading the supplied image.** Its bright ridges form a graphene-like cone. The crossing near $k_y=0$ is the [Dirac point](../../../dirac-point.md), not in general the [Fermi level](../../../fermi-level.md). In the paper's plotted [energy](../../../energy-split.md) coordinates its [energy](../../../energy-split.md) is roughly $E_D\sim1.4$–$1.5\,\mathrm{eV}$. A velocity follows from a branch slope independently of the [energy](../../../energy-split.md) zero:

$$
v=\frac1\hbar\left|\frac{dE}{dk_y}\right|,\qquad 1\,\mathrm{eV\,\mathring A}/\hbar=1.519\times10^5\,\mathrm{m\,s^{-1}}.
$$

For example, the lower branch moves by about $0.3\,\mathrm{eV}$ between $|k_y|\sim0.03$ and $0.11\,\mathrm{\mathring A^{-1}}$. This gives $dE/dk\sim3.8\,\mathrm{eV\,\mathring A}$ and

$$
\boxed{v_F\sim6\times10^5\,\mathrm{m\,s^{-1}}\quad\text{as a rough linear-cone estimate}.}
$$

Reading other points changes the estimate by tens of percent. The original exam image has unequal [energy](../../../energy-split.md) increments on nearly equally spaced labelled ticks, so it does not justify a precise fitted velocity. The value is an estimate of the cone slope extrapolated to the Fermi crossing, rather than a measured derivative exactly at a visibly identified Fermi cutoff.

To determine a [Fermi energy](../../../fermi-energy.md), first calibrate the Fermi edge, then subtract the chosen reference [energy](../../../energy-split.md). Neither a Fermi-level marker nor an explicit energy-zero convention is supplied in this crop. If its upper termination near $1.9\,\mathrm{eV}$ is intended to represent the Fermi cutoff, the conditional graph answer is **$E_F\simeq1.9\,\mathrm{eV}$ on that axis**, or **$E_F-E_D\sim0.4\,\mathrm{eV}$** relative to the Dirac crossing. Identifying the crossing itself as the [Fermi energy](../../../fermi-energy.md) would incorrectly assume undoped [graphene](../../../graphene.md).

The research article cited by the exam identifies this as linearly polarized [graphene](../../../graphene.md) [ARPES](../../../angle-resolved-photoemission-spectroscopy.md) and independently states $E_F-E_D\simeq0.4\,\mathrm{eV}$ for the substrate-doped sample. That resolves the relative [energy](../../../energy-split.md) when this external calibration is admitted.[Section 3, printed p.2 and figure 1(b): [Dirac point](../../../dirac-point.md) below the [Fermi energy](../../../fermi-energy.md)](https://hrg.pusan.ac.kr/articles/JPCM_0953-8984_26_33_335501.pdf) **The crop alone does not uniquely fix an absolute [Fermi energy](../../../fermi-energy.md)**; the source-supported relative value and the conditional $1.9\,\mathrm{eV}$ axis reading should be distinguished.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2017](../../2017-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)

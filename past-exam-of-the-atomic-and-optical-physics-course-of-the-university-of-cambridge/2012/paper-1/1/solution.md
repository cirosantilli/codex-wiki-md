<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [condensate wavefunction](../../../../condensate-wavefunction.md) convention $\int |\psi|^2\,d^3r=N$, so $n(\mathbf r)=|\psi(\mathbf r)|^2$ is the [number density](../../../../number-density.md) and $\psi/\sqrt N$ is a normalized one-particle orbital. The [contact interaction](../../../../contact-interaction-quantum-mechanics.md) strength is $U_0=4\pi\hbar^2a/m$ for dilute atoms with [s-wave scattering length](../../../../s-wave-scattering-length.md) $a$. The [chemical potential](../../../../chemical-potential-split.md) $\mu=\partial E/\partial N$ fixes the stationary time dependence $e^{-i\mu t/\hbar}$ and enforces normalization when minimizing the [energy](../../../../energy-split.md). The [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md) follows from an [energy functional](../../../../energy-functional.md) that contains the pair-counting factor $1/2$:

$$
E[\psi]=\int\left[\frac{\hbar^2}{2m}|\nabla\psi|^2+V|\psi|^2+\frac{U_0}{2}|\psi|^4\right]d^3r.
$$

Varying $E-\mu\int|\psi|^2d^3r$ gives the stationary [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md); the interaction contribution to that equation is $U_0 n\psi$, without the factor $1/2$.

For the broadening discussed here assume **repulsive interactions**, $a>0$. The [Thomas–Fermi approximation for a condensate](../../../../thomas-fermi-approximation-for-a-condensate.md) neglects the [gradient](../../../../gradient.md) [kinetic energy](../../../../kinetic-energy.md) compared with the trapping and interaction [energies](../../../../energy-split.md). At fixed spatial scale, increasing $N U_0$ increases the mean-field potential. Expansion then reduces the [kinetic energy](../../../../kinetic-energy.md) further: for a cloud radius $R$, its scale per atom is $\hbar^2/(mR^2)$, whereas the trap [energy](../../../../energy-split.md) scale is $m\omega^2R^2$. Their ratio decreases as $(a_0/R)^4$. In the weak-interaction limit the [kinetic energy](../../../../kinetic-energy.md) instead balances confinement, giving the [Gaussian wave packet](../../../../gaussian-wave-packet.md) [ground state](../../../../ground-state.md) of the [quantum harmonic oscillator](../../../../quantum-harmonic-oscillator-split.md).

The [spherical Thomas–Fermi condensate](../../../../spherical-thomas-fermi-condensate.md) has

$$
 n_{\rm TF}(r)=\frac{\mu-\tfrac12m\omega^2r^2}{U_0}\quad(0\leq r\leq R),\qquad n_{\rm TF}(r)=0\quad(r>R),\qquad \mu=\tfrac12m\omega^2R^2.
$$

Integrating this [density](../../../../density.md) gives $N=8\pi\mu R^3/(15U_0)$. Thus

$$
\boxed{R=a_0(15Na/a_0)^{1/5},\qquad \mu_{\rm TF}=\frac{\hbar\omega}{2}(15Na/a_0)^{2/5}.}
$$

At fixed $N$, stronger repulsion produces a wider, lower [wavefunction](../../../../wave-function-split.md): the [Gaussian wave packet](../../../../gaussian-wave-packet.md) crosses over towards the [square root](../../../../square-root.md) of an inverted [parabola](../../../../parabola.md), with an almost flat central region and a steeper outer drop. The _[density](../../../../density.md)_ is the inverted [parabola](../../../../parabola.md); the _[wavefunction](../../../../wave-function-split.md)_ is its [square root](../../../../square-root.md). The exact [wavefunction](../../../../wave-function-split.md) remains smooth and has a tail, since [kinetic energy](../../../../kinetic-energy.md) cannot be neglected near the [Thomas–Fermi condensate edge rounding](../../../../thomas-fermi-condensate-edge-rounding.md) region. The [healing length](../../../../healing-length.md) must be small compared with the cloud size in the bulk. Attractive interactions would not follow this large-$N$ expansion argument.

The original plot compares the noninteracting endpoint with two normalized repulsive [spherical Thomas–Fermi condensate](../../../../spherical-thomas-fermi-condensate.md) profiles. The latter are asymptotic shapes, rather than exact intermediate solutions of the [Gross–Pitaevskii equation](../../../../gross-pitaevskii-equation.md). Each has the same integrated atom number; $\chi=Na/a_0$ labels the illustrative interaction strengths.

<a id="1/image-condensate-broadening"></a>
![](../../../../past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2012/paper-1-condensate-profiles.png)

**[Figure 1](#1/image-condensate-broadening). Condensate broadening**.

Choose $A$ real and positive. The [Gaussian integral](../../../../gaussian-integral.md) gives

$$
N=A^2\pi^{3/2}a_0^3,\qquad
\boxed{A=\frac{\sqrt N}{\pi^{3/4}a_0^{3/2}},\quad \mu_0=\frac32\hbar\omega,\quad E_0=\frac32N\hbar\omega.}
$$

The three [zero-point energies](../../../../zero-point-energy.md) add for each atom. The ideal-gas [chemical potential](../../../../chemical-potential-split.md) is a one-atom [energy](../../../../energy-split.md); the total [energy](../../../../energy-split.md) includes all $N$ atoms.

For weak interactions, the first-order correction in [perturbation theory](../../../../perturbation-theory.md) is the [energy functional](../../../../energy-functional.md) of the [contact interaction](../../../../contact-interaction-quantum-mechanics.md) evaluated on the unperturbed [Gaussian wave packet](../../../../gaussian-wave-packet.md). The [integral](../../../../integral-split.md) needed is

$$
\int |\psi_0|^4d^3r=\frac{N^2}{\pi^3a_0^6}\left(\frac{\pi a_0^2}{2}\right)^{3/2}=\frac{N^2}{(2\pi)^{3/2}a_0^3}.
$$

Consequently the [Gaussian interaction energy of a trapped condensate](../../../../gaussian-interaction-energy-of-a-trapped-condensate.md) is

$$
\boxed{E_I=\frac{N^2U_0}{2(2\pi)^{3/2}a_0^3},\qquad \frac{E_I}{\hbar\omega}=\frac{N^2a}{\sqrt{2\pi}\,a_0}.}
$$

Here $\hbar\omega=\hbar^2/(ma_0^2)$. These are the mean-field expressions consistent with the supplied equation and $\int|\psi|^2=N$. Exact first-order [perturbation theory](../../../../perturbation-theory.md) for precisely $N$ atoms in one orbital replaces $N^2$ by $N(N-1)$ through the number of distinct pairs; this distinction is negligible in the large-$N$ regime of the crossover estimate.

To judge the ideal-gas approximation, compare the interaction [energy](../../../../energy-split.md) with the _total_ ideal [energy](../../../../energy-split.md), or compare the interaction [energy](../../../../energy-split.md) per atom with $\hbar\omega$:

$$
\frac{E_I}{E_0}=\frac{2}{3\sqrt{2\pi}}\frac{Na}{a_0}.
$$

Thus the [crossover from Gaussian to Thomas–Fermi condensate](../../../../crossover-from-gaussian-to-thomas-fermi-condensate.md) is governed by $\chi=Na/a_0$: [perturbation theory](../../../../perturbation-theory.md) is reliable for $\chi\ll1$, while the regime of the [Thomas–Fermi approximation for a condensate](../../../../thomas-fermi-approximation-for-a-condensate.md) requires $\chi\gg1$. **The characteristic crossover number is $N_c\sim a_0/a$; there is no sharp critical atom number here.** If one specifically defines crossover by $E_I=E_0$ using the weak-interaction expression, it gives $N_c=(3\sqrt{2\pi}/2)a_0/a$. That prefactor is a convention-dependent estimate extrapolated to the edge of [perturbation theory](../../../../perturbation-theory.md), not a phase transition. Comparing $E_I$ itself to a single $\hbar\omega$ would incorrectly omit a factor of $N$.

For the numerical estimate use $m\simeq87\times1.66054\times10^{-27}\,\mathrm{kg}$ and $\hbar\simeq1.05457\times10^{-34}\,\mathrm{J\,s}$. Then

$$
a_0=\sqrt{\frac{\hbar}{m(2\pi\times50\,\mathrm{s^{-1}})}}\simeq1.52\,\mathrm{\mu m},\qquad
\boxed{N_c\sim\frac{a_0}{a}\simeq3.0\times10^2\ \text{atoms}.}
$$

The particular equality $E_I=E_0$ would instead give about $1.15\times10^3$ atoms. These quantify different choices within a smooth crossover; a well-developed [spherical Thomas–Fermi condensate](../../../../spherical-thomas-fermi-condensate.md) profile requires going substantially beyond the characteristic scale.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the atomic and Optical Physics course of the University of Cambridge](../../../split.md)
5. [Atomic and Optical Physics course of the University of Cambridge](../../../../atomic-and-optical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

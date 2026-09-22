<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a free-space [electric dipole transition](../../../../electric-dipole-transition.md), the [spontaneous emission](../../../../spontaneous-emission.md) rate in SI units is

$$
\boxed{\Gamma=\frac{\omega_0^3|\mathbf d|^2}{3\pi\epsilon_0\hbar c^3}
\ \propto\ |d|^2\omega_0^3.}
$$

Here $|\mathbf d|^2$ includes the relevant dipole components; a specified single polarization requires its corresponding [matrix element](../../../../matrix-element.md).

A complete scattering cycle returns the internal state to the [ground state](../../../../ground-state.md) and changes the atomic [momentum](../../../../momentum-split.md) to $\mathbf P+\mathbf p-\mathbf p'$. Thus

$$
\boxed{\Delta E=\frac{|\mathbf P+\mathbf p-\mathbf p'|^2-P^2}{2M}
=\frac{\mathbf P\cdot(\mathbf p-\mathbf p')}{M}
+\frac{|\mathbf p-\mathbf p'|^2}{2M}.}
$$

For [photon-scattering recoil heating](../../../../photon-scattering-recoil-heating.md) with isotropic emission of fixed [momentum](../../../../momentum-split.md) magnitude, $\langle\mathbf p'\rangle=0$, giving

$$
\boxed{\langle\Delta E\rangle_{\rm em}
=\frac{\mathbf P\cdot\mathbf p}{M}+\frac{p^2}{2M}+\frac{p'^2}{2M}.}
$$

The first term is the velocity-dependent [work](../../../../work.md) of absorption and can cool an atom if the [photon](../../../../photon.md) opposes its motion. The last two are positive absorption and emission [recoil](../../../../recoil.md) energies. If the actual absorbed directions are also isotropic and independent of $\mathbf P$, the first term averages to zero. For approximately equal incoming and outgoing [photon](../../../../photon.md) momenta $\hbar k$,

$$
\boxed{\langle\Delta E\rangle=2E_R,\qquad E_R=\frac{\hbar^2k^2}{2M}.}
$$

Isotropic incident illumination alone would not guarantee isotropic absorption if Doppler-dependent excitation selected directions.

**Source qualification for the trapped calculation.** Set $m=M$ for the same atom. The printed Gaussian $\exp[-x^2/(2l_0)^2]$ has the wrong width for the specified [harmonic oscillator](../../../../simple-harmonic-motion.md): the printed ground and first-excited functions have squared norms $\sqrt2$ and $2\sqrt2$, respectively. The normalized oscillator states fixed by the given $l_0=\sqrt{\hbar/(m\omega_{\rm HO})}$ instead use

$$
\psi_0=\pi^{-1/4}l_0^{-1/2}e^{-x^2/(2l_0^2)},\qquad
\psi_1=\sqrt2(x/l_0)\psi_0.
$$

Also, one common complex phase multiplying both off-diagonal terms does not make the [Hamiltonian](../../../../hamiltonian.md) a [Hermitian operator](../../../../hermitian-operator.md). Use an absorption [matrix element](../../../../matrix-element.md) $(\hbar\Omega/2)e^{-ikx}$ and its [Hermitian conjugate](../../../../hermitian-conjugation.md) for emission; choosing the opposite propagation convention reverses the imaginary sideband phase but not a [transition probability](../../../../transition-probability.md). The physical results below use these explicitly stated corrections. Parts (i) and (ii) also give the literal integrals of the printed functions.

**[Conditional motional heating and recoil averaging](../../../../conditional-motional-heating-and-recoil-averaging.md).** With $\eta=kl_0/\sqrt2$, an oscillator [eigenstate](../../../../eigenstate.md) has $\langle K\rangle_n=\langle V\rangle_n=(n+1/2)\hbar\omega_{\rm HO}/2$. Therefore the absorption outcomes have

$$
\boxed{0\to0:\ \Delta K=\Delta V=0;\qquad
0\to1:\ \Delta K=\Delta V=\hbar\omega_{\rm HO}/2.}
$$

The same statements hold for the specified emission outcomes $|e,0\rangle\to|g,0\rangle$ and $|e,0\rangle\to|g,1\rangle$. Internal excitation [energy](../../../../energy-split.md) goes into, or comes from, the [photon](../../../../photon.md) and is distinct from this external [energy](../../../../energy-split.md) change. Emission into the first motional state makes the emitted [photon](../../../../photon.md) correspondingly less energetic.

A sudden [recoil](../../../../recoil.md) from $|0\rangle$ gives probabilities $P_n=e^{-\eta^2}\eta^{2n}/n!$, so $P_1\simeq\eta^2\ll1$ while $P_0\simeq1$. The rare first sideband transfers a whole trap quantum, much larger than $E_R$; the mean is nevertheless

$$
\boxed{\sum_n P_n\,n\hbar\omega_{\rm HO}
=\eta^2\hbar\omega_{\rm HO}=E_R.}
$$

The emission average is the same for a one-dimensional [recoil](../../../../recoil.md) of the same magnitude. Projecting isotropic three-dimensional emission onto one axis instead gives a factor $\langle\cos^2\theta\rangle=1/3$ for that axis.

A sudden unobserved kick initially raises [kinetic energy](../../../../kinetic-energy.md) by $E_R$ and leaves the position distribution, hence [potential energy](../../../../potential-energy.md), unchanged. It creates a coherent [superposition](../../../../superposition-principle.md) of motional states. The equal kinetic/potential increments above concern energy-eigenstate-conditioned outcomes, or time-averaged/dephased motion; these are different measurement conditions. There is no contradiction.

With $\Gamma>\omega_{\rm HO}$, motional sidebands are not cleanly resolved, and a short-lived excited atom has little time to move before decay. In the stronger sudden limit $\Gamma\gg\omega_{\rm HO}$ the recoil-kick picture is direct. For only the stated inequality, finite linewidth weights can change numerical factors; it does not fix an exact continuous-wave scattering rate. **The average heating remains of [recoil](../../../../recoil.md) order per absorption or emission**, and of order $2E_R$ when both absorption and emission kicks are counted at full magnitude. For the axial component of isotropic three-dimensional emission, the emission contribution instead carries the factor $1/3$ noted above. Strong confinement suppresses the chance of changing $n$, but does not make its averaged [recoil energy](../../../../recoil-energy.md) disappear. This agrees with free-space [recoil](../../../../recoil.md) heating while replacing small continuous [energy](../../../../energy-split.md) changes by rare quantized motional changes.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
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

<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a uniform nearest-neighbour [harmonic chain](../../../../../harmonic-chain.md) with [displacement](../../../../../displacement.md) $u_j$, conjugate [momentum](../../../../../momentum-split.md) $p_j$, mass $m_0$, [spring](../../../../../spring.md) stiffness $\kappa$, lattice spacing $a$ and periodic length $\ell=Na$. These specify a standard model for the requested notes, not additional numerical exam data. Its [Lagrangian](../../../../../lagrangian.md) and [Hamiltonian](../../../../../hamiltonian.md) are

$$
L=\sum_j\left[\frac{m_0}{2}\dot u_j^2-\frac\kappa2(u_{j+1}-u_j)^2\right],\qquad H=\sum_j\left[\frac{p_j^2}{2m_0}+\frac\kappa2(u_{j+1}-u_j)^2\right].
$$

Variation gives $m_0\ddot u_j=\kappa(u_{j+1}-2u_j+u_{j-1})$. For a mode $e^{i(kja-\omega t)}$, periodicity requires $k=2\pi n/\ell$ and

$$
\boxed{\omega_k=2\sqrt{\kappa/m_0}\,|\sin(ka/2)|.}
$$

The lattice makes $k$ periodic modulo $2\pi/a$, so choose one [Brillouin zone](../../../../../brillouin-zone.md). At long wavelength $\omega_k\simeq v|k|$, where $v=a\sqrt{\kappa/m_0}$ is the [sound speed](../../../../../speed-of-sound.md). The [continuum limit of a harmonic chain](../../../../../continuum-limit-of-a-harmonic-chain.md) expands $u_{j+1}-u_j\simeq a\partial_xu$ and replaces $\sum_j$ by $a^{-1}\int dx$. Defining [mass density](../../../../../density.md) $\rho=m_0/a$ and one-dimensional elastic coefficient $K=\kappa a$ gives

$$
L=\int_0^\ell dx\left[\frac\rho2(\partial_tu)^2-\frac K2(\partial_xu)^2\right],\qquad \rho\partial_t^2u-K\partial_x^2u=0,\qquad v^2=K/\rho.
$$

The [momentum](../../../../../momentum-split.md) density is $\Pi=\rho\partial_tu$, and the [Hamiltonian](../../../../../hamiltonian.md) density is $\Pi^2/(2\rho)+K(\partial_xu)^2/2$. Translational invariance of $u$ makes total [momentum](../../../../../momentum-split.md) conserved. The continuum approximation describes acoustic wavelengths large compared with $a$; it is not a justification for extending the lattice dispersion and zero-point sums to arbitrarily large [wavevector](../../../../../wavevector.md).[chapter 4, §4.1.1, printed pp.103–105: periodic monatomic chain and acoustic dispersion](../../../../../applications-of-quantum-mechanics-by-david-tong.md)

[canonical quantization](../../../../../canonical-quantization.md) promotes the coordinates and momenta to operators with $[u_j,p_l]=i\hbar\delta_{jl}$ and the other equal-time [commutators](../../../../../commutator.md) zero. In the continuum, $[u(x),\Pi(x')]=i\hbar\delta_{\rm per}(x-x')$. The nonzero [normal modes](../../../../../normal-mode.md) can be represented by independent [phonon](../../../../../phonon.md) operators obeying $[b_k,b_q^\dagger]=\delta_{kq}$. A useful lattice expansion is

$$
u_j=X+\frac1{\sqrt N}\sum_{k\ne0}\sqrt{\frac{\hbar}{2m_0\omega_k}}\left(b_ke^{ikja}+b_k^\dagger e^{-ikja}\right),
$$

where $X=N^{-1}\sum_j u_j$ is the centre-of-mass [displacement](../../../../../displacement.md). The corresponding [momentum](../../../../../momentum-split.md) is

$$
p_j=\frac PN-\frac i{\sqrt N}\sum_{k\ne0}\sqrt{\frac{m_0\hbar\omega_k}{2}}\left(b_ke^{ikja}-b_k^\dagger e^{-ikja}\right),\qquad [X,P]=i\hbar.
$$

Including the centre-of-mass term restores the full site [commutator](../../../../../commutator.md): the nonzero-mode sum alone gives $i\hbar(\delta_{jl}-1/N)$. Substitution diagonalizes the [Hamiltonian](../../../../../hamiltonian.md),

$$
\boxed{H=\frac{P^2}{2Nm_0}+\sum_{k\ne0}\hbar\omega_k(b_k^\dagger b_k+\tfrac12).}
$$

A [phonon](../../../../../phonon.md) is one quantum of a collective [normal mode](../../../../../normal-mode.md), carrying energy $\hbar\omega_k$ and lattice [momentum](../../../../../momentum-split.md) $\hbar k$ modulo a reciprocal-lattice [vector](../../../../../vector.md). Reality of $u_j$ relates its Fourier coordinates by $u_k^\dagger=u_{-k}$; it does not remove the independent oppositely travelling [phonon](../../../../../phonon.md) modes. Using one complete [Brillouin zone](../../../../../brillouin-zone.md) avoids double-counting real standing-wave coordinates.[§4.1.4, quantization of lattice vibrations](../../../../../applications-of-quantum-mechanics-by-david-tong.md)

The free [centre of mass](../../../../../center-of-mass.md) has no restoring force and must not be treated as an oscillator of zero frequency. Fixing it, weakly pinning it, or specifying a finite centre-of-mass volume defines the corresponding zero-mode factor. With a fixed [centre of mass](../../../../../center-of-mass.md), the internal thermal [partition function](../../../../../canonical-partition-function.md) and occupations are

$$
Z_{\rm int}=\prod_{k\ne0}\frac1{2\sinh(\beta\hbar\omega_k/2)},\qquad \langle n_k\rangle=\frac1{e^{\beta\hbar\omega_k}-1}.
$$

The internal energy is $\sum_{k\ne0}\hbar\omega_k(\langle n_k\rangle+1/2)$; its high-temperature [heat capacity](../../../../../heat-capacity.md) approaches $(N-1)k_B$. For a large one-dimensional chain at [temperatures](../../../../../temperature-split.md) below the lattice cutoff but above its finite-size mode spacing,

$$
\frac{U_T}{\ell}=\int\frac{dk}{2\pi}\frac{\hbar v|k|}{e^{\beta\hbar v|k|}-1}=\frac{\pi(k_BT)^2}{6\hbar v},\qquad \frac C\ell=\frac{\pi k_B^2T}{3\hbar v}.
$$

This [one-dimensional acoustic phonon heat capacity](../../../../../one-dimensional-acoustic-phonon-heat-capacity.md) shows that **quantization turns classical normal waves into bosonic excitations with a linear low-temperature [heat capacity](../../../../../heat-capacity.md) in one dimension**. The Euclidean field action $S_E=\tfrac12\int_0^{\beta\hbar}d\tau\,dx\,[\rho(\partial_\tau u)^2+K(\partial_xu)^2]$ is Gaussian, with periodic imaginary-time boundary conditions; its Fourier modes reproduce these oscillators. Absolute [displacement](../../../../../displacement.md) correlations require the zero-mode convention, and the lattice regulates short-distance fluctuations.

## ↑ Ancestors (14)

1. [A](../a.md)
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

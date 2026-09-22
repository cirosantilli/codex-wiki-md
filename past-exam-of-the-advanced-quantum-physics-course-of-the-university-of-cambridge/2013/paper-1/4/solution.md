<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Define $\hbar\omega_0=E_2-E_1$ and use [radiation energy density](../../../../radiation-energy-density.md) $u(\omega)$ per unit [angular frequency](../../../../angular-frequency.md), excluding the zero-point contribution. The [Angular-frequency Einstein coefficients](../../../../angular-frequency-einstein-coefficients.md) give rates per atom: $B_{12}u(\omega_0)$ for absorption, $B_{21}u(\omega_0)$ for [stimulated emission](../../../../stimulated-emission.md), and $A_{21}$ for [spontaneous emission](../../../../spontaneous-emission.md). Stimulated emission adds a photon to the stimulating mode; spontaneous emission persists with no incident photons.

<a id="4/image-absorption-stimulated-emission-and-spontaneous-emission-between-two-nondegenerate-levels"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2013/paper-1-aqp2013-radiative-transitions.png)

**[Figure 3](#4/image-absorption-stimulated-emission-and-spontaneous-emission-between-two-nondegenerate-levels). Absorption, stimulated emission and spontaneous emission between two nondegenerate levels**. [Source](paper-1-aqp2013-radiative-transitions.py).

In thermal equilibrium the [Boltzmann distribution](../../../../boltzmann-distribution.md) gives $N_2/N_1=e^{-\hbar\omega_0/(k_{\rm B}T)}$. Balancing up and down rates yields

$$
N_1B_{12}u=N_2(A_{21}+B_{21}u),\qquad
u=\frac{A_{21}}{B_{12}e^{\hbar\omega_0/(k_{\rm B}T)}-B_{21}}.
$$

Matching the [Planck law](../../../../planck-s-law.md) for every temperature fixes

$$
\boxed{B_{12}=B_{21},\qquad\frac{A_{21}}{B_{21}}=\frac{\hbar\omega_0^3}{\pi^2c^3}.}
$$

No degeneracy factor is needed for these nondegenerate levels.[§4.3.2, printed pp.123–127: thermal balance and Einstein coefficients](../../../../topics-in-quantum-mechanics-by-david-tong.md)

For plates of large area $A$ and spacing $d$, the surviving low-frequency [transverse electromagnetic mode](../../../../transverse-electromagnetic-mode.md) has one polarization, $\mathbf E\parallel\hat{\mathbf z}$, and in-plane [wavevector](../../../../wavevector.md). Periodic in-plane counting gives

$$
dN=\frac{A}{(2\pi)^2}\,2\pi k\,dk,\qquad
\frac1{Ad}\frac{dN}{d\omega}=\frac{\omega}{2\pi c^2d}.
$$

Multiplying this [single-polarization two-dimensional photon density of states](../../../../single-polarization-two-dimensional-photon-density-of-states.md) by $\hbar\omega$ and the [Bose-Einstein distribution](../../../../bose-einstein-distribution.md) produces the [thermal radiation between parallel conducting plates](../../../../thermal-radiation-between-parallel-conducting-plates.md):

$$
\boxed{u_{\rm plates}(\omega)=\frac{\hbar\omega^2}{2\pi c^2d}\frac1{e^{\hbar\omega/(k_{\rm B}T)}-1}.}
$$

The same rate balance therefore gives

$$
\left(\frac AB\right)_{\rm plates}=\frac{\hbar\omega_0^2}{2\pi c^2d},\qquad
\boxed{\frac{(A/B)_{\rm plates}}{(A/B)_{\rm free}}=\frac{\pi c}{2\omega_0d}\gg1.}
$$

These $B$ coefficients refer to the radiation polarization in their respective environments: isotropic free-space $B$ must not automatically be equated to the coefficient for a specified $z$-polarized field.

For [hydrogen](../../../../hydrogen.md), take the quantization axis along $z$, neglect [spin-orbit coupling](../../../../spin-orbit-interaction.md), and assume perfect plates, a wide in-plane region and an unmodified atomic wavefunction: $a_{\rm B}\ll d\ll c/\omega_0$, with negligible surface-induced mixing or shifts. The [electric-dipole selection rules for hydrogen](../../../../electric-dipole-selection-rules-for-hydrogen.md) require $\Delta l=\pm1$; the allowed $z$ field has $\Delta m_\ell=0$. Hence the [polarization-selective spontaneous emission between conducting plates](../../../../polarization-selective-spontaneous-emission-between-conducting-plates.md) gives

$$
\boxed{m_\ell=0:\quad A_{\rm plates}\sim A_{\rm free}\frac{c}{\omega_0d},\qquad
\tau_{\rm plates}\sim\tau_{\rm free}\frac{\omega_0d}{c}.}
$$

The [thin-cavity enhancement of a normal electric dipole](../../../../thin-cavity-enhancement-of-a-normal-electric-dipole.md) applies: the $2p_0\to1s$ dipole points along $z$ and couples to the enhanced mode density. For $m_\ell=\pm1$, the transition dipoles lie in the $x$–$y$ plane and couple to none of these low-frequency modes: **the electric-dipole decay rate is zero in the ideal model**, so this channel's lifetime is infinite. Real finite, imperfect plates and additional decay or mixing channels limit the lifetime. The order-one orientation factor for the allowed transition does not change the requested lifetime scaling.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

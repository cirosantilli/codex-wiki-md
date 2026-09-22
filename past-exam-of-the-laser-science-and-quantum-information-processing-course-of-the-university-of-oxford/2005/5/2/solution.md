<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A resonant [Rabi pi pulse](../../../../rabi-pi-pulse.md) satisfies $\Omega T_\pi=\pi$. The supplied $T_\pi=0.256\,\mathrm s$ therefore gives

$$
\boxed{\Omega=\frac\pi{0.256\,\mathrm s}\simeq12.27\,\mathrm{rad\,s^{-1}},\qquad
\frac\Omega{2\pi}=1.953125\,\mathrm{Hz}.}
$$

The ideal rotating-frame operation is $-iX$, a [Pauli X gate](../../../../pauli-x-gate.md) up to [global phase](../../../../global-phase.md).

Both logical states belong to the electronic ground level. A fast [electric dipole transition](../../../../electric-dipole-transition.md) between them is forbidden, and spontaneous radiative relaxation at a hyperfine radiofrequency is weak. The optical readout field is off during the coherent pulse. Neglecting relaxation is therefore consistent with a population lifetime much longer than $0.256\,\mathrm s$. Magnetic noise, collisions and technical dephasing are additional limitations; the ideal coherent calculation assumes their effects are small over this interval.

At detuning $\delta$, define $\Omega_{\rm eff}=\sqrt{\Omega^2+\delta^2}$. The same two-level [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) gives

$$
P_b(t)=\frac{\Omega^2}{\Omega^2+\delta^2}
\sin^2\left(\frac{t\sqrt{\Omega^2+\delta^2}}2\right).
$$

For an accurate fixed-duration $\pi$ rotation, the detuning must be small compared with the [Rabi angular frequency](../../../../rabi-angular-frequency.md). Writing $\delta\nu=\delta/(2\pi)$,

$$
\boxed{|\delta\nu|\ll\frac\Omega{2\pi}=1.95\,\mathrm{Hz},}
$$

a fractional mismatch much smaller than $6.1\times10^{-9}$ relative to the $320.7\,\mathrm{MHz}$ carrier. This is an accuracy scale, not an assertion that a particular nonzero detuning gives a perfect gate.

The [small-detuning error of a Rabi pi pulse](../../../../small-detuning-error-of-a-rabi-pi-pulse.md) quantifies a chosen tolerance. For an initial $|a\rangle$ and the resonant pulse duration,

$$
1-P_b(T_\pi)=\left(\frac\delta\Omega\right)^2+O\!\left((\delta/\Omega)^4\right).
$$

A population-transfer error at most $\epsilon$ consequently requires approximately **$|\delta\nu|\lesssim1.95\sqrt\epsilon\,\mathrm{Hz}$**; for example, **about $0.20\,\mathrm{Hz}$ for one percent error**. Full gate calibration also includes pulse area and drive phase, beyond this population-transfer criterion.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [5](../../5-split.md)
3. [2005](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

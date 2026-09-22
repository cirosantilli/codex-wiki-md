# Harmonic vibrational energy levels

↑ **Parent:** [Diatomic bond stretch](diatomic-bond-stretch.md)

Quantizing the stretching coordinate gives a [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) with [reduced mass](reduced-mass.md) $\mu$:

$$
\widehat H=V_0-\frac{\hbar^2}{2\mu}\frac{d^2}{dq^2}+\frac12kq^2,\qquad
E_v=V_0+\hbar\omega\left(v+\frac12\right),\qquad
v=0,1,2,\ldots.
$$

Here $v$ is the vibrational [quantum number](quantum-number.md) and $\hbar=h/(2\pi)$ the reduced [Planck constant](planck-constant.md). Consecutive [energy eigenvalues](energy-eigenvalue-split.md) have gap $\hbar\omega$; the [ground state](ground-state.md) has [zero-point energy](zero-point-energy.md) $\hbar\omega/2$ above the well minimum. The offset $V_0$ cancels from every transition [energy](energy-split.md).

<a id="image-diatomic-stretch-potential-and-quantum-levels"></a>
![](diatomic-stretch-potential-and-quantum-levels.png)

**[Figure 9](#image-diatomic-stretch-potential-and-quantum-levels). Local harmonic approximation near a potential minimum and equally spaced vibrational energy eigenvalues**. Original dimensionless model with $x=q/\sqrt{\hbar/(\mu\omega)}$ and $e=(E-V_0)/(\hbar\omega)$. The blue parabola is $x^2/2$; levels are $e=v+1/2$. The orange comparison is the stipulated [Morse potential](morse-potential.md) $8(1-e^{-x/4})^2$, with the same curvature at $x=0$; it is not a fit to [hydrogen chloride](hydrogen-chloride.md). Arrows show adjacent vibrational gaps, with [molecular rotation](molecular-rotation.md) omitted.

A short proof uses [creation and annihilation operators](creation-and-annihilation-operators.md): with $\ell=\sqrt{\hbar/(\mu\omega)}$, write $q=\ell(a+a^\dagger)/\sqrt2$. The [Quantum Hamiltonian](hamiltonian-quantum-mechanics.md) becomes $\widehat H-V_0=\hbar\omega(a^\dagger a+1/2)$. Nonnegativity of $a^\dagger a$ gives the lowest level; repeated application of $a^\dagger$ raises its [energy](energy-split.md) by $\hbar\omega$ each time. This also gives $\langle q\rangle_v=0$ and

$$
\langle q^2\rangle_v=\frac{\hbar}{\mu\omega}\left(v+\frac12\right).
$$

The [ground state](ground-state.md) therefore has a nonzero spread of [bond lengths](bond-length.md), even though its mean stretching [displacement](displacement.md) vanishes. A stationary [energy eigenstate](energy-eigenstate.md) has a time-independent position [probability density](probability-density.md); the classical [oscillation](oscillation.md) curve is not a trajectory of an [atomic nucleus](atomic-nucleus-split.md) in that state.

The parabolic model formally extends $q$ to the whole [real line](real-line.md), whereas an actual [bond length](bond-length.md) satisfies $r>0$. It is useful for low levels concentrated near $r_e$, with typical stretching [displacements](displacement.md) much smaller than $r_e$. It fails near breakup of the [chemical bond](chemical-bond-split.md) and when neglected [anharmonicity](anharmonicity.md) becomes substantial.

## ↑ Ancestors (5)

1. [Diatomic bond stretch](diatomic-bond-stretch.md)
2. [Molecular vibration](molecular-vibration.md)
3. [Molecule](molecule-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [University of Florida HCl and DCl FTIR experiment](university-of-florida-hcl-and-dcl-ftir-experiment.md)

<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [quantum dense coding](../../../../../superdense-coding.md), a shared [Bell pair](../../../../../bell-pair.md) lets Alice send two classical [bits](../../../../../bit.md) by transmitting one [qubit](../../../../../qubit.md). Use [photon polarization](../../../../../photon-polarization.md) as the [computational basis](../../../../../computational-basis.md), $|0\rangle=|H\rangle$, $|1\rangle=|V\rangle$, and define the [Bell states](../../../../../bell-state-split.md)

$$
|\phi^\pm\rangle=\frac{|00\rangle\pm|11\rangle}{\sqrt2},\qquad
|\psi^\pm\rangle=\frac{|01\rangle\pm|10\rangle}{\sqrt2}.
$$

Alice and Bob initially share $|\phi^+\rangle_{AB}$. Alice encodes a two-[bit](../../../../../bit.md) message $(m,n)$ by applying the [Pauli operator](../../../../../pauli-operator.md) $X^nZ^m$ to her [qubit](../../../../../qubit.md):

$$
\begin{array}{c|c|c}
(m,n)&\text{Alice's operation}&\text{shared state}\\\hline
(0,0)&I&|\phi^+\rangle\\
(1,0)&Z&|\phi^-\rangle\\
(0,1)&X&|\psi^+\rangle\\
(1,1)&XZ&-|\psi^-\rangle
\end{array}
$$

The last minus sign is a [global phase](../../../../../global-phase.md). Alice transmits her [photon](../../../../../photon.md) to Bob, who now holds both [qubits](../../../../../qubit.md) and uses a [Bell-basis measurement](../../../../../bell-basis-measurement.md) to identify the message. The four [Bell states](../../../../../bell-state-split.md) are [orthogonal](../../../../../orthogonal-vectors.md), so an ideal [Bell state analyzer](../../../../../bell-state-analyzer.md) decodes them without error. The resource cost is one previously shared [Bell pair](../../../../../bell-pair.md) and one transmitted [qubit](../../../../../qubit.md) per two classical [bits](../../../../../bit.md); the shared [quantum entanglement](../../../../../entangled-state.md) is consumed. Before transmission Bob's [reduced density matrix](../../../../../reduced-density-matrix.md) is $I/2$ for every message, consistent with the [no-communication theorem](../../../../../no-communication-theorem.md).

The [BBO](../../../../../beta-barium-borate.md) crystal supplies the [polarization-entangled photon pair](../../../../../polarization-entangled-photon-pair.md). An ultraviolet [laser](../../../../../laser-split.md) pumps this [nonlinear optical crystal](../../../../../nonlinear-optical-crystal.md); [spontaneous parametric down-conversion](../../../../../spontaneous-parametric-down-conversion.md) produces signal and idler [photons](../../../../../photon.md) with $\omega_p=\omega_s+\omega_i$ and [phase matching](../../../../../phase-matching.md) $\mathbf k_p=\mathbf k_s+\mathbf k_i$. In a noncollinear [type-II phase matching](../../../../../type-ii-phase-matching.md) arrangement, collect the intersections of the two emission cones. The alternatives $|H\rangle_A|V\rangle_B$ and $|V\rangle_A|H\rangle_B$ must be indistinguishable in arrival time, spectrum and spatial mode. Compensation of [birefringence](../../../../../birefringence.md) and adjustment of the [relative quantum phase](../../../../../relative-quantum-phase.md) then give $(|HV\rangle+|VH\rangle)/\sqrt2$; a local [Pauli X gate](../../../../../pauli-x-gate.md) converts it to $|\phi^+\rangle$. [Half-wave plates](../../../../../half-wave-plate.md) and other [waveplates](../../../../../waveplate.md) implement Alice's [Pauli gates](../../../../../pauli-gate.md). The [BBO](../../../../../beta-barium-borate.md) is the pair source; the message is encoded subsequently by the local optical elements.[1995, Figures 1 and 2: intersecting type-II emission cones and compensation; Table I: four Bell states](../../../../../new-high-intensity-source-of-polarization-entangled-photon-pairs-by-paul-g-kwiat-and-others.md)

A basic passive [linear optics](../../../../../linear-optics.md) [Bell state analyzer](../../../../../bell-state-analyzer.md) with no extra resources identifies only two of the four polarization [Bell states](../../../../../bell-state-split.md) unambiguously. Thus the ideal two-[bit](../../../../../bit.md) capacity presupposes complete [Bell-basis measurement](../../../../../bell-basis-measurement.md); that basic optical implementation alone does not attain it deterministically.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [7 and 8](../../../7-and-8-split.md)
4. [2005](../../../split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

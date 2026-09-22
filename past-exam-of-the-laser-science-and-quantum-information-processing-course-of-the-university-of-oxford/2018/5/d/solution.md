<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In heteronuclear [liquid-state NMR quantum computing](../../../../liquid-state-nmr-quantum-computing.md), different [gyromagnetic ratios](../../../../gyromagnetic-ratio.md) give well-separated resonance [frequencies](../../../../frequency.md). A resonant transverse radio-frequency pulse selects one nucleus; its [phase](../../../../phase-waves.md) sets the rotation axis in the transverse plane and its duration and [amplitude](../../../../wave-amplitude.md) set the rotation angle. Detuning, free precession and rotating-frame [phase](../../../../phase-waves.md) changes supply $z$ rotations. For homonuclear [spins](../../../../spin.md), differing [chemical shifts](../../../../chemical-shift.md) can provide [frequency](../../../../frequency.md) selectivity, but selective pulses must be narrow enough not to rotate the other [spin](../../../../spin.md). Exactly magnetically equivalent [spins](../../../../spin.md) cannot be independently addressed by a spatially uniform radio-frequency field merely because they are labelled as different [qubits](../../../../qubit.md).

In the weak-coupling regime, the secular [NMR scalar coupling](../../../../nmr-scalar-coupling.md) is

$$
H_J=2\pi\hbar J I_{1z}I_{2z}=\frac{\pi\hbar J}{2}Z_1Z_2,
$$

with $J$ in hertz. Free coupling evolution for $1/(2|J|)$ gives an entangling propagator $\exp[-i\operatorname{sgn}(J)\pi Z_1Z_2/4]$. Suitable single-qubit $z$ rotations convert it to a [Controlled-Z gate](../../../../controlled-z-gate.md), and Hadamard conjugation on the target converts controlled-$Z$ to a [controlled-NOT gate](../../../../controlled-not-gate.md). Refocusing pulses remove unwanted Zeeman evolution and unwanted couplings. This construction applies to resolved, weakly coupled homonuclear [spins](../../../../spin.md) as well as heteronuclear [spins](../../../../spin.md); strongly coupled or equivalent [spins](../../../../spin.md) need a different control analysis.

These controls supply a universal gate set on a finite addressable connected register, but conventional liquid-state molecular [NMR](../../../../nuclear-magnetic-resonance-split.md) is not an architecture that scales straightforwardly to arbitrary register size. A finite chemical-shift bandwidth causes spectral crowding as more [spins](../../../../spin.md) and coupling-split transitions are added; increasingly selective pulses become slow relative to coherence times, and complicated coupling networks require extensive refocusing. The exponentially small pseudo-pure-state signal further limits the complete ensemble scheme. Formal unitary universality therefore does not establish scalable physical addressability, gate speed or initialization.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

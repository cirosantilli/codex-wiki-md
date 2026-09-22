<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [liquid-state NMR quantum computing](../../../../liquid-state-nmr-quantum-computing.md), use two distinguishable spin-$1/2$ [atomic nuclei](../../../../atomic-nucleus-split.md) in one molecule as the two [qubits](../../../../qubit.md). Their different resonance [frequencies](../../../../frequency.md) permit selective radiofrequency pulses for one-[qubit](../../../../qubit.md) rotations. In a suitable rotating frame, refocusing removes unwanted one-spin terms while the [NMR scalar coupling](../../../../nmr-scalar-coupling.md) supplies

$$
H_J=2\pi\hbar J I_zS_z=\frac{\pi\hbar J}{2}Z_1Z_2.
$$

Assuming $J>0$, free evolution for $t=1/(2J)$ implements $U_J=e^{-i\pi Z_1Z_2/4}$. Define $R_z(\theta)=e^{-i\theta Z/2}$. Then

$$
\boxed{\mathrm{CZ}=e^{-i\pi/4}
[R_z(-\pi/2)\otimes R_z(-\pi/2)]U_J.}
$$

This equality follows directly by evaluating the four diagonal entries: the first three are $+1$ and the $11$ entry is $-1$. Negative $J$ can be handled by refocusing or reversing the effective interaction sign. The [global phase](../../../../global-phase.md) can be ignored.

Thus the [marked-state phase oracle](../../../../marked-state-phase-oracle.md) for $11$ requires scalar-coupling evolution and calibrated one-spin rotations. For a marked word $b_1b_2$, conjugate by $X_1^{1-b_1}X_2^{1-b_2}$, realized as selective $\pi$ pulses. The [Grover diffusion operator](../../../../grover-diffusion-operator.md) uses the same entangling operation with additional one-[qubit](../../../../qubit.md) pulses. [Liquid-state NMR quantum computing](../../../../liquid-state-nmr-quantum-computing.md) usually reads an ensemble signal and often prepares an effective pseudo-pure deviation from a large mixed background; that reproduces this small [quantum algorithm](../../../../quantum-algorithm.md)'s signal without providing a scalable source of pure initialized [qubits](../../../../qubit.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

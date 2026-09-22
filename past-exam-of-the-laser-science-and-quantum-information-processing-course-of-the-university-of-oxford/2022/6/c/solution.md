<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S$ denote immediate transmission through the BS1 subsystem between Bob's lower-right port and Alice's upper-left port; let $L$ denote transmission after one visit to each internal mirror. From the same [beam splitter](../../../../beam-splitter.md) rules as in [b](../b.md), the corresponding amplitudes in either direction are

$$
S=c,\qquad L=-c^3
$$

up to a common fixed two-mirror propagation phase. The minus sign in $L$ comes from the $1'\to1$ or reverse $1\to1'$ scattering. The two paths selected by D0's time gate are $L$ on the outward journey followed by $S$ on the return, and $S$ outward followed by $L$ on the return. They have the same total delay and fixed propagation phase, so their [probability amplitudes](../../../../probability-amplitude.md) interfere.

For the first history, Alice applies $e^{i\phi_A}$ to the late component, while Bob's return-time modulation is not encountered in the return delay arm. For the second, Alice's early component is unmodulated and Bob applies $e^{i\phi_B}$ in the return delay arm. Bob must time his modulation to the return passage, leaving the outward reference preparation unchanged; this is implicit in the stated encoding. Each enabled modulator is traversed twice, so its $\pi/2$ single-pass [phase](../../../../phase-waves.md) becomes the stipulated $\pi$.

Include the amplitude $c$ to enter BS1 through BS2, and the amplitude of modulus $c$ to reach D0 through BS2 on return. Both histories therefore contain six 50:50 [beam splitter](../../../../beam-splitter.md) factors. Ignoring one common unobservable [global phase](../../../../global-phase.md),

$$
\mathcal A_{D0}=-c^6(e^{i\phi_A}+e^{i\phi_B})
=-\frac18(e^{i\phi_A}+e^{i\phi_B}).
$$

Hence the **unconditional probability per emitted [photon](../../../../photon.md)**, with no renormalization after discarding paths, is

$$
\boxed{P(D0\mid\phi_A,\phi_B)
=\frac{1+\cos(\phi_A-\phi_B)}{32}
=\frac1{16}\cos^2\!\frac{\phi_A-\phi_B}{2}.}
$$

For the allowed values $0,\pi$, this is $1/16$ when $\phi_A=\phi_B$ and zero otherwise. The ignored trajectories exit other ports or other time bins; excluding them from D0's acceptance does not increase the success probability. Equal mirror reflection phases, channel phases and Alice's mirror phase multiply both accepted histories equally and cancel from the [interference](../../../../interference-wave-propagation.md) condition. A residual _relative_ phase would need calibration.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
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

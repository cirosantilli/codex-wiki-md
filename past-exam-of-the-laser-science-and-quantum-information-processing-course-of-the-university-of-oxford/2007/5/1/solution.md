<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Represent the [single-photon state](../../../../single-photon-state.md) by its two path [probability amplitudes](../../../../probability-amplitude.md). The first [Hadamard gate](../../../../hadamard-gate.md) sends $|0\rangle$ to $(|0\rangle+|1\rangle)/\sqrt2$. With $P(\phi)=\operatorname{diag}(1,e^{i\phi})$ for the lower-arm [phase shifter](../../../../phase-shifter.md), the complete [Mach-Zehnder interferometer](../../../../mach-zehnder-interferometer.md) gives

$$
H P(\phi)H|0\rangle
=\frac{1+e^{i\phi}}2|0\rangle+\frac{1-e^{i\phi}}2|1\rangle
=e^{i\phi/2}\left(\cos\frac\phi2|0\rangle-i\sin\frac\phi2|1\rangle\right).
$$

The [global phase](../../../../global-phase.md) has no effect on detection. By the [Born rule](../../../../born-rule.md),

$$
\boxed{P_0(\phi)=\cos^2\frac\phi2,\qquad P_1(\phi)=\sin^2\frac\phi2.}
$$

They sum to one. At $\phi=0$, port 1 is a [dark port](../../../../dark-port.md); at $\phi=\pi$, the roles reverse. The result uses coherent addition of the path amplitudes, rather than addition of separate path [probabilities](../../../../probability.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [5](../../5-split.md)
3. [2007](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

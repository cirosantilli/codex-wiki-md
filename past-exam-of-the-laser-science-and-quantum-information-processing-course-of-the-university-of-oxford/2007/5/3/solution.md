<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Calibrate the two-Hadamard [Mach-Zehnder interferometer](../../../../mach-zehnder-interferometer.md) so that the passive box leaves no relative [wave phase](../../../../phase-waves.md) or path disturbance. Then $H^2|0\rangle=|0\rangle$, and port 1 is dark. A photon at port 1 is therefore impossible for the passive box under these assumptions.

For an active ideal detector in arm 1, the first [Hadamard gate](../../../../hadamard-gate.md) prepares $(|0\rangle+|1\rangle)/\sqrt2$. Absorption, which triggers the detector, has probability $1/2$. On a no-absorption outcome, the surviving unnormalized state is $|0\rangle/\sqrt2$. Applying the second Hadamard gives

$$
H\frac{|0\rangle}{\sqrt2}=\frac{|0\rangle+|1\rangle}{2}.
$$

Its squared norm is $1/2$, the survival probability; normalizing it earlier and forgetting that probability would overcount successful trials. The unconditional outcomes for an active detector are

$$
\boxed{P(\text{absorption})=\frac12,\quad
P(\text{port }0)=\frac14,\quad P(\text{port }1)=\frac14.}
$$

Thus **a port-1 click identifies an active detector without triggering it**, with **single-pass success probability $1/4$**, conditional on testing an active device. A port-0 click is inconclusive. Among trials in which the photon survives, half are successful, but that conditional fraction is not the single-pass success probability.

This is the [balanced Hadamard interaction-free measurement](../../../../balanced-hadamard-interaction-free-measurement.md) version of the [Elitzur-Vaidman bomb tester](../../../../elitzur-vaidman-bomb-tester.md). Conditioning on no absorption changes the [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md) available for recombination; a calibrated dark-port click reveals that change. An uncontrolled phase shift in the passive arm could also brighten the port, so the inference depends on the stated optical calibration. It does not assign an observed classical trajectory to the photon before detection. If the same active device is retested after inconclusive clicks, the [repeated weak-rotation bomb-test efficiency](../../../../repeated-weak-rotation-bomb-test-efficiency.md) gives eventual success $(1/4)/(1-1/4)=1/3$; the requested single pass remains $1/4$.

## ↑ Ancestors (12)

1. [3](../3.md)
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

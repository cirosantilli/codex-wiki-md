<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [parallel LC circuit](../../../../parallel-lc-circuit.md) both components have the same voltage [phasor](../../../../phasor.md). Adding their current [phasors](../../../../phasor.md) by [Kirchhoff's current law](../../../../kirchhoff-node-law.md) gives the total [electrical admittance](../../../../electrical-admittance.md):

$$
\frac1Z=\frac1{j\omega L}+j\omega C
=j\left(\omega C-\frac1{\omega L}\right).
$$

Thus

$$
\boxed{Z=\frac{j\omega L}{1-\omega^2LC},\qquad
|Z|=\frac{\omega L}{|1-\omega^2LC|},\qquad
\arg Z=\begin{cases}+\pi/2,&\omega<1/\sqrt{LC},\\-\pi/2,&\omega>1/\sqrt{LC}.\end{cases}}
$$

At the ideal parallel [resonance](../../../../resonance.md), $\omega_0=1/\sqrt{LC}$, the two branch current [phasors](../../../../phasor.md) cancel. The net [electrical admittance](../../../../electrical-admittance.md) is zero and the magnitude of the [complex impedance](../../../../electrical-impedance.md) tends to infinity: the parallel combination behaves as an open circuit at that [frequency](../../../../frequency.md). Its [complex argument](../../../../argument-complex-analysis.md) is undefined exactly at the pole. Finite component losses replace the infinite peak by a large finite [electrical impedance](../../../../electrical-impedance.md). This conclusion concerns a voltage-driven sinusoidal response; an ideal resonant current drive does not have a bounded sinusoidal steady-state voltage.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the $e^{i\omega t}$ [phasor](../../../../phasor.md) convention and interpret [impedance matching](../../../../impedance-matching.md) as conjugate matching for the [maximum power transfer theorem](../../../../maximum-power-transfer-theorem.md). The load [electrical impedance](../../../../electrical-impedance.md) of the [series circuit](../../../../series-circuit.md) is

$$
Z_{RC}=R-\frac{i}{\omega C}.
$$

For $Z=A+i\omega B$, the condition $Z_{RC}=Z^*$ equates the [real parts](../../../../real-part.md) and [imaginary parts](../../../../imaginary-part.md):

$$
\boxed{R=A,\qquad \omega^2BC=1,\qquad \omega=\frac1{\sqrt{BC}}.}
$$

These formulas require $B>0$, $C>0$ and a passive realization with $A\geq0$, evaluated at the matching [angular frequency](../../../../angular-frequency.md); if $A,B$ depend on $\omega$, the equation for $\omega$ is implicit.

There is a convention ambiguity in the word “matched”. Literal equality $Z_{RC}=Z$, as required for equal bridge arms in part (b), instead gives $R=A$ and $\omega^2BC=-1$, requiring $B<0$. The inductive cases below use conjugate matching; literal equality is impossible for either passive inductive configuration at a finite positive [angular frequency](../../../../angular-frequency.md) because its [electrical reactance](../../../../electrical-reactance.md) is positive while that of the [series RC impedance](../../../../series-rc-impedance.md) is negative.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

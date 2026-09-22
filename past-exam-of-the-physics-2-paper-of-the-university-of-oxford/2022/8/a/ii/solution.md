<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [electrical resistance](../../../../../electrical-resistance.md) $R_p>0$ in a [parallel circuit](../../../../../parallel-circuit.md) with [inductance](../../../../../inductance.md) $L>0$, add [electrical admittances](../../../../../electrical-admittance.md) and invert:

$$
Z=\left(\frac1{R_p}+\frac1{i\omega L}\right)^{-1}
=\frac{R_p\omega^2L^2}{R_p^2+\omega^2L^2}
+i\omega\frac{R_p^2L}{R_p^2+\omega^2L^2}.
$$

Conjugate [impedance matching](../../../../../impedance-matching.md) to the [series RC impedance](../../../../../series-rc-impedance.md) requires

$$
\frac1{\omega C}=\frac{\omega R_p^2L}{R_p^2+\omega^2L^2},
\qquad R_p^2=\omega^2L(CR_p^2-L).
$$

It is possible at a finite positive [angular frequency](../../../../../angular-frequency.md) exactly when $CR_p^2>L$, in which case

$$
\boxed{\omega=\frac{R_p}{\sqrt{L(CR_p^2-L)}},\qquad R=\frac{L}{CR_p}.}
$$

The expression for $R$ follows by substituting this $\omega^2$ into the [real part](../../../../../real-part.md) of $Z$. If $CR_p^2\leq L$, no such finite matching [angular frequency](../../../../../angular-frequency.md) exists. Under literal equality, both passive inductive configurations fail by the sign of their [imaginary parts](../../../../../imaginary-part.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the physics 2 paper of the University of Oxford](../../../../split.md)
6. [Physics 2 paper of the University of Oxford](../../../../../physics-2-paper-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

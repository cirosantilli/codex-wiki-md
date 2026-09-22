<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use sinusoidal [phasors](../../../../phasor.md) with physical values $v(t)=\operatorname{Re}(\widehat V e^{j\omega t})$, $i(t)=\operatorname{Re}(\widehat I e^{j\omega t})$, and $j^2=-1$. The [complex impedance](../../../../electrical-impedance.md) is $Z=\widehat V/\widehat I=X+jY$: its [modulus](../../../../modulus.md) is the voltage-to-current [amplitude](../../../../wave-amplitude.md) ratio, and its [complex argument](../../../../argument-complex-analysis.md) is the voltage-minus-current [phase difference](../../../../phase-difference.md). Here $X$ is the [electrical resistance](../../../../electrical-resistance.md) part and $Y$ the signed [electrical reactance](../../../../electrical-reactance.md); the source's $X,Y$ notation differs from the common $R,X$ notation.

The component laws $v_R=Ri$, $v_L=L\,di/dt$ and $i_C=C\,dv_C/dt$ give the [complex impedances](../../../../electrical-impedance.md) of an ideal [resistor](../../../../resistor.md), [inductor](../../../../inductor.md) and [capacitor](../../../../capacitor.md):

$$
Z_R=R,\qquad Z_L=j\omega L,\qquad Z_C=\frac1{j\omega C}=-\frac j{\omega C}.
$$

In a [series circuit](../../../../series-circuit.md) the same [electric current](../../../../electric-current.md) flows through both components, so [Kirchhoff's voltage law](../../../../kirchhoff-cycle-law.md) adds their voltage [phasors](../../../../phasor.md). The resulting [series RC impedance](../../../../series-rc-impedance.md) is

$$
Z=R-\frac j{\omega C},\qquad
\boxed{|Z|=\sqrt{R^2+\frac1{\omega^2C^2}},\qquad
\arg Z=-\arctan\frac1{\omega CR}.}
$$

For positive $R,C,\omega$, the negative [phase difference](../../../../phase-difference.md) means that [electric current](../../../../electric-current.md) leads the applied [electric potential difference](../../../../electric-potential-difference.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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

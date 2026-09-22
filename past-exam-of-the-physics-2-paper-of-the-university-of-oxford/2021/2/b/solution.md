<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A suitable [electrical circuit](../../../../electrical-circuit-split.md) has $R$ in series with the input and a shunt branch consisting of $C$ in parallel with the lossy [inductor](../../../../inductor.md) $R_L+i\omega L$; take the output [voltage](../../../../voltage.md) across that shunt branch. This is the middle arrangement in the circuit figure. In terms of its [complex impedance](../../../../electrical-impedance.md),

$$
Z_p=\left(i\omega C+\frac1{R_L+i\omega L}\right)^{-1},\qquad H(\omega)=\frac{U_2}{U_1}=\frac{Z_p}{R+Z_p}.
$$

At [direct current](../../../../direct-current.md) the [capacitor](../../../../capacitor.md) is an [open circuit](../../../../open-circuit.md) and the [inductor](../../../../inductor.md) contributes only $R_L$, so $H(0)=R_L/(R+R_L)=0.01$. Therefore

$$
\boxed{R=99\,\Omega.}
$$

When $R_L$ is neglected, $Z_p=i\omega L/(1-\omega^2LC)$. At the [antiresonance](../../../../antiresonance.md) $\omega_0^2LC=1$ its [electrical admittance](../../../../electrical-admittance.md) vanishes, so $|H|$ reaches its maximum value of one. Consequently

$$
\boxed{C=\frac1{L\omega_0^2}=1.78\times10^{-3}\,\mathrm F.}
$$

This value uses precisely the requested lossless approximation; keeping $R_L$ changes both the peak position and its height. A [transfer function](../../../../transfer-function.md) peak and one DC measurement do not uniquely identify every possible [two-port network](../../../../two-port-network.md), but the displayed arrangement meets both observations to the stipulated approximation. Also, the angle brackets in the source must denote AC [wave amplitudes](../../../../wave-amplitude.md) or [root mean square](../../../../root-mean-square.md) values: the literal time averages of sinusoidal [voltages](../../../../voltage.md) are zero, whose ratio would be undefined.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

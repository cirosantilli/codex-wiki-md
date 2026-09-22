<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the source's top terminal have [voltage](../../../../voltage.md) [phasor](../../../../phasor.md) $V_0$ and its bottom terminal zero. Denote the left and right junctions by $L$ and $R$. The two left [resistors](../../../../resistor.md) are equal, so at balance $V_L=V_0/2$. Zero [electric current](../../../../electric-current.md) through the [ammeter](../../../../ammeter.md) requires $V_R=V_L$, and therefore equal upper and lower right-arm [electrical impedances](../../../../electrical-impedance.md):

$$
Z=\frac{R_x}{1+i\omega R_xC_x}=W,\qquad
W=R_v+\frac1{i\omega C}=R_v-\frac{i}{\omega C}.
$$

Write $x=\omega R_xC_x$. Separating [real parts](../../../../real-part.md) and [imaginary parts](../../../../imaginary-part.md) gives

$$
R_v=\frac{R_x}{1+x^2},\qquad
\frac1{\omega C}=\frac{\omega R_x^2C_x}{1+x^2}.
$$

The second equation implies $1+x^2=\omega^2R_x^2CC_x$. Subtract $x^2=\omega^2R_x^2C_x^2$ to obtain

$$
\boxed{\omega_0=\frac1{R_x\sqrt{C_x(C-C_x)}},\qquad
\frac{C_x}{C}=1-\frac{R_v}{R_x}.}
$$

A finite balance with positive components requires $0<C_x<C$, and then $0<R_v<R_x$. This [equal-ratio RC bridge](../../../../equal-ratio-rc-bridge.md) uses equality of arm [electrical impedances](../../../../electrical-impedance.md), independent of the conjugate-matching convention in part (a).

**Detector convention.** The stated negligible-[electrical impedance](../../../../electrical-impedance.md) [ammeter](../../../../ammeter.md) is an ideal [short circuit](../../../../short-circuit.md), whose actual terminal [voltage](../../../../voltage.md) is zero at every [angular frequency](../../../../angular-frequency.md). The nontrivial bridge output usually intended is the _open-circuit_ junction difference, obtained with the detector removed or replaced by a high-[input impedance](../../../../input-impedance.md) [voltmeter](../../../../voltmeter.md). Define its polarity by

$$
V_{\rm oc}=V_R-V_L
=V_0\left(\frac{W}{Z+W}-\frac12\right)
=\frac{V_0(W-Z)}{2(W+Z)}.
$$

For a detector of finite [electrical impedance](../../../../electrical-impedance.md) $Z_A$, its terminal [voltage](../../../../voltage.md) is instead

$$
V_A=V_{\rm oc}\frac{Z_A}{Z_A+Z_{\rm th}},\qquad
Z_{\rm th}=\frac R2+\frac{ZW}{Z+W}.
$$

Here $Z_{\rm th}$ is the [Thévenin equivalent](../../../../thevenin-equivalent.md) [electrical impedance](../../../../electrical-impedance.md), found by shorting the ideal source. This exhibits why the ideal-[ammeter](../../../../ammeter.md) limit $Z_A\to0$ has zero terminal [voltage](../../../../voltage.md) even when the bridge is unbalanced.

## ↑ Ancestors (12)

1. [B](../b.md)
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

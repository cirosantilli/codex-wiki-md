<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an [ideal operational amplifier](../../../../ideal-operational-amplifier.md) under [negative feedback](../../../../negative-feedback.md), the grounded non-inverting terminal makes the inverting terminal a [virtual ground](../../../../virtual-ground.md), and no [electric current](../../../../electric-current.md) enters either input. The feedback [resistor](../../../../resistor.md) and [capacitor](../../../../capacitor.md) have parallel [electrical impedance](../../../../electrical-impedance.md)

$$
Z_f=\left(\frac1{R_2}+i\omega C\right)^{-1}=\frac{R_2}{1+i\omega R_2C}.
$$

[Kirchhoff's current law](../../../../kirchhoff-node-law.md) at the inverting node gives $\widetilde V_i/R_1+\widetilde V_o/Z_f=0$, and hence

$$
\boxed{\frac{\widetilde V_o}{\widetilde V_i}=-\frac{R_2/R_1}{1+i\omega R_2C}.}
$$

With the stated components, $R_2C=16.0\,\mu\mathrm s$ and $R_2/R_1=5$. Thus this [inverting low-pass amplifier](../../../../inverting-low-pass-amplifier.md) has exactly the same ideal [cutoff frequency](../../../../cutoff-frequency.md) and normalized [frequency response](../../../../frequency-response.md) as the passive [RC low-pass filter](../../../../rc-low-pass-filter.md), with output multiplied by $-5$:

$$
\boxed{V_o(t)=-\frac{5V_{i0}}{\sqrt{1+(\omega\tau)^2}}\cos\!\left(\omega t-\tan^{-1}(\omega\tau)\right).}
$$

Its [amplitude](../../../../wave-amplitude.md) ratios at the three stated [frequencies](../../../../frequency.md) are $4.99975$, $3.52616$, and $0.97560$. One principal choice of [phase shift](../../../../phase-shift.md) is $180^\circ-\tan^{-1}(\omega\tau)$: respectively $179.424^\circ$, $134.848^\circ$, and $101.252^\circ$. Adding or subtracting $360^\circ$ describes the same output; the extra inversion must be retained.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [voltage divider](../../../../voltage-divider.md) relation for the [capacitor](../../../../capacitor.md) output gives the [transfer function](../../../../transfer-function.md)

$$
H(\omega)=\frac{V_{\rm out}}{V_{\rm in}}=\frac{1/(i\omega C)}{R+i\omega L+1/(i\omega C)}=\boxed{\frac1{1-\omega^2LC+i\omega RC}.}
$$

Consequently the relative [wave amplitude](../../../../wave-amplitude.md) is

$$
\boxed{|H|=\frac1{\sqrt{(1-\omega^2LC)^2+(\omega RC)^2}}.}
$$

For input $V_0\cos\omega t$, the output is $V_0|H|\cos(\omega t+\phi)$, where the continuous [phase shift](../../../../phase-shift.md) is

$$
\boxed{\phi=-\operatorname{atan2}(\omega RC,\,1-\omega^2LC).}
$$

For positive [frequency](../../../../frequency.md) and $R>0$, this [phase shift](../../../../phase-shift.md) goes from $0$ towards $-\pi$, passing through $-\pi/2$ at $\omega_0$. A one-argument arctangent without a quadrant correction would wrongly predict a positive [phase shift](../../../../phase-shift.md) above $\omega_0$. The [capacitor](../../../../capacitor.md) follows a slowly varying input [voltage](../../../../voltage.md), while its output falls as $1/(\omega^2LC)$ at high [frequency](../../../../frequency.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
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

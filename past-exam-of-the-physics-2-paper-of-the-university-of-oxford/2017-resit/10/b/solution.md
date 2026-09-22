<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original diagram's upper arm is a series [resistor](../../../../resistor.md) and [capacitor](../../../../capacitor.md); its lower arm is a parallel [resistor](../../../../resistor.md) and [capacitor](../../../../capacitor.md). The output is the upper-minus-lower [voltage](../../../../voltage.md) across that parallel arm. Assume an ideal input voltage source and an unloaded output. Their [electrical impedances](../../../../electrical-impedance.md) are

$$
Z_s=R+\frac1{i\omega C},\qquad Z_p=\frac{R}{1+i\omega RC}.
$$

For this [series-parallel RC band-pass filter](../../../../series-parallel-rc-band-pass-filter.md), the [voltage divider](../../../../voltage-divider.md) gives, with $w=\omega RC$,

$$
\boxed{H(\omega)=\frac{\widetilde V_{\rm out}}{\widetilde V_{\rm in}}
=\frac{Z_p}{Z_s+Z_p}
=\frac1{3+i(w-w^{-1})}
=\frac{iw}{1-w^2+3iw}.}
$$

Taking the real part of $V_0H e^{i\omega t}$ yields the steady output

$$
\boxed{V_{\rm out}(t)=\frac{V_0}{\sqrt{9+(w-w^{-1})^2}}
\cos\!\left[\omega t-\arctan\!\left(\frac{w-w^{-1}}3\right)\right].}
$$

Initial charging contributes decaying transients if the source is switched on at a finite time; the displayed expression is the sinusoidal steady state. The output polarity matters: reversing the indicated output [voltage](../../../../voltage.md) would multiply $H$ by $-1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

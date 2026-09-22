<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positive [angular frequency](../../../../angular-frequency.md), the squared [amplitude](../../../../wave-amplitude.md) response of the [series-parallel RC band-pass filter](../../../../series-parallel-rc-band-pass-filter.md) is

$$
|H|^2=\frac1{9+(w-w^{-1})^2}.
$$

Its denominator is minimized exactly when $w=w^{-1}$, so

$$
\boxed{\omega_0=\frac1{RC},\qquad H(\omega_0)=\frac13,\qquad
V_{\rm out}(t)=\frac{V_0}{3}\cos\omega_0t.}
$$

This is a [band-pass filter](../../../../band-pass-filter.md) maximum produced entirely by the two RC arms; the drawn [electrical circuit](../../../../electrical-circuit-split.md) contains no [inductor](../../../../inductor.md). The low- and high-[frequency](../../../../frequency.md) limits are

$$
\boxed{H\simeq i\omega RC\quad(\omega\ll\omega_0),\qquad
H\simeq-\frac{i}{\omega RC}\quad(\omega\gg\omega_0).}
$$

Thus the output [amplitude](../../../../wave-amplitude.md) tends to zero linearly with $\omega$ at low [frequency](../../../../frequency.md) and as $1/\omega$ at high [frequency](../../../../frequency.md). In real time,

$$
V_{\rm out}\simeq-V_0\omega RC\sin\omega t\quad(\omega\ll\omega_0),\qquad
V_{\rm out}\simeq\frac{V_0}{\omega RC}\sin\omega t\quad(\omega\gg\omega_0).
$$

The upper series [capacitor](../../../../capacitor.md) suppresses low [frequencies](../../../../frequency.md), while the lower shunt [capacitor](../../../../capacitor.md) suppresses high [frequencies](../../../../frequency.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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

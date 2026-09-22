<h1 id="11b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The PDF gives initial position $(x',y',z')=(1,0,0)$ and initial rotating-frame [velocity](../../../../../../velocity.md) zero. Use those values; the TeX erroneously places dots over the position coordinates.

For rotation about the third axis, the supplied acceleration relation and [Newton's second law](../../../../../../newton-s-second-law.md) give the [equations of motion in a rotating frame](../../../../../../equation-of-motion-in-a-rotating-frame.md)

$$
\ddot x'-2\omega\dot y'+3\omega^2x'=0,\qquad
\ddot y'+2\omega\dot x'+3\omega^2y'=0,\qquad
\ddot z'+4\omega^2z'=0.
$$

Thus $z'=0$. Set $\zeta=x'+iy'$ to combine the planar equations:

$$
\ddot\zeta+2i\omega\dot\zeta+3\omega^2\zeta=0.
$$

The two characteristic roots are $i\omega$ and $-3i\omega$. From $\zeta(0)=1$ and $\dot\zeta(0)=0$,

$$
\zeta=\frac34e^{i\omega t}+\frac14e^{-3i\omega t}.
$$

The triple-angle formulas therefore give the particularly simple [astroid motion of a harmonic oscillator in a rotating frame](../../../../../../astroid-motion-of-a-harmonic-oscillator-in-a-rotating-frame.md)

$$
\boxed{x'=\cos^3(\omega t),\qquad
y'=\sin^3(\omega t),\qquad z'=0.}
$$

The orbit satisfies $|x'|^{2/3}+|y'|^{2/3}=1$; the zero [speed](../../../../../../speed.md) at each cusp is consistent with the smooth time-parametrized motion.

Its rotating-frame [speed](../../../../../../speed.md) is

$$
|\boldsymbol v'|^2
=9\omega^2\sin^2(\omega t)\cos^2(\omega t)
=\frac94\omega^2\sin^2(2\omega t).
$$

Hence, for $\omega>0$, **the first maximum occurs at $t=\pi/(4\omega)$**, and

$$
\boxed{v'_{\max}=\frac32\omega.}
$$

The maximum repeats periodically. For a signed negative angular frequency, use $\pi/(4|\omega|)$ and $3|\omega|/2$; at $\omega=0$ the particle remains at rest.

<a id="11b/ii/image-astroid-orbit-and-the-first-maximum-speed-in-the-rotating-frame"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-4-rotating-astroid.png)

**[Figure 2](#11b/ii/image-astroid-orbit-and-the-first-maximum-speed-in-the-rotating-frame). Astroid orbit and the first maximum speed in the rotating frame**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11B](../../11b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

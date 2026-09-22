<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $h,g\in Y$, their product $hg$ is holomorphic and integrable on the disk by the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md). Its angular mean on every centered circle is $h(0)g(0)$ by the [mean value property](../../../../mean-value-property-for-harmonic-functions.md). Polar integration therefore gives

$$
\langle h,\overline g\rangle=\int_Dh(z)g(z)\,dA(z)
=\pi h(0)g(0).
$$

If $g(0)=0$, this vanishes for every $h\in Y$, proving $\boxed{Z\subseteq Y^\perp}$. Integrability of the product justifies integration over the full disk, even when the individual [holomorphic functions](../../../../holomorphic-function-split.md) grow near its boundary.

The inclusion is **strict**. Set $w(z)=|z|^2-1/2$, a nonzero bounded function in $L^2(D)$. For every $h\in Y$,

$$
\langle w,h\rangle
=2\pi\overline{h(0)}\int_0^1(r^2-1/2)r\,dr=0.
$$

Thus $w\in Y^\perp$. It cannot equal $\overline g$ for holomorphic $g$: equality almost everywhere between these [continuous functions](../../../../continuous-function.md) would give equality everywhere, making $g=w$ a real-valued nonconstant [holomorphic function](../../../../holomorphic-function-split.md), which is impossible. Therefore

$$
\boxed{Z\ne Y^\perp.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

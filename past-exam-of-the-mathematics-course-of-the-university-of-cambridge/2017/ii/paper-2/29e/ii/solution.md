<h1 id="29e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The horizontal contribution is $B(x)=(2\pi)^{-1}\int_{-\pi}^{\pi}e^{-ix\sin z}e^{i\nu z}\,dz$. The two nondegenerate stationary points of the phase $-\sin z$ are $\pi/2$ and $-\pi/2$, with second [derivatives](../../../../../../derivative.md) $1$ and $-1$. The [stationary phase method](../../../../../../stationary-phase-method.md) gives their contributions

$$
\frac1{\sqrt{2\pi x}}\left(e^{-ix+i\nu\pi/2+i\pi/4}+e^{ix-i\nu\pi/2-i\pi/4}\right)
=\sqrt{\frac2{\pi x}}\cos\left(x-\frac{\nu\pi}2-\frac\pi4\right),
$$

with remainder $O(x^{-3/2})$ for smooth fixed amplitudes localized near the stationary points. On the remaining portions, use [integration by parts](../../../../../../integration-by-parts.md). The endpoint term is

$$
\frac1{2\pi}\left[\frac{e^{-ix\sin z+i\nu z}}{-ix\cos z}\right]_{-\pi}^{\pi}
=\frac{\sin(\pi\nu)}{\pi x}.
$$

Cutoff endpoints cancel between pieces; a second integration gives the other nonstationary contributions $O(x^{-2})$. Thus this endpoint term cancels the leading vertical term. Altogether

$$
\boxed{f_\nu(x)=\sqrt{\frac2{\pi x}}\cos\left(x-\frac{\nu\pi}2-\frac\pi4\right)+O(x^{-3/2}),\qquad a=\frac32.}
$$

This [stationary phase endpoint cancellation in a half-strip contour](../../../../../../stationary-phase-endpoint-cancellation-in-a-half-strip-contour.md) is necessary: omitting it would leave an erroneous $x^{-1}$ remainder for noninteger $\nu$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [29E](../../29e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

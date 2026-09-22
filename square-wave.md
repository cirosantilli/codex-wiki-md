# Square wave

↑ **Parent:** [Fourier series](fourier-series-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_wave)

A [square wave](square-wave.md) alternates between two constant levels for equal halves of a [period](period-of-a-function.md). Choose a $2\pi$-periodic [function](function-split.md) equal to $1$ on $(0,\pi)$ and $-1$ on $(-\pi,0)$, with value zero at the jumps. Its [odd function](odd-function.md) symmetry makes the mean and every cosine [Fourier coefficient](fourier-coefficient.md) vanish. Directly integrating the two constant pieces gives

$$
a_0=a_n=0,\qquad b_n=\frac{2[1-(-1)^n]}{\pi n},\qquad
f(x)\sim\frac4\pi\sum_{k=0}^{\infty}\frac{\sin((2k+1)x)}{2k+1}.
$$

Thus only [odd](odd-function.md) sine [Fourier harmonics](fourier-harmonic.md) occur, with amplitudes decreasing like the reciprocal of their frequency multiplier. Every finite [Fourier partial sum](fourier-partial-sum.md) is smooth, yet their [pointwise limit](pointwise-limit.md) has jumps. At those jumps the [Fourier series](fourier-series-split.md) converges to zero, the midpoint of the two levels, regardless of which value we assign to the original [function](function-split.md) there.

This example explains how smooth components can encode sharp transitions. Increasing the number of [Fourier harmonics](fourier-harmonic.md) narrows the transition region, but also produces the persistent overshoot described by the [Gibbs phenomenon](gibbs-phenomenon.md). The illustrated square wave and coefficient calculation are mathematical constructions, not measurements of a physical device.

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Fourier partial sum](fourier-partial-sum.md)
- [Fourier series](fourier-series-split.md)
- [Gibbs phenomenon](gibbs-phenomenon.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/14e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/2/solution.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [Square wave](square-wave.md)

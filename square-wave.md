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

**Table of contents**

- [Harmonic power of a square wave](harmonic-power-of-a-square-wave.md)

## ↑ Ancestors (5)

1. [Fourier series](fourier-series-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Fourier partial sum](fourier-partial-sum.md)
- [Fourier series](fourier-series-split.md)
- [Gibbs phenomenon](gibbs-phenomenon.md)
- [Harmonic power of a square wave](harmonic-power-of-a-square-wave.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/14e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/2/solution.md)
- [Solution](past-exam-of-the-physics-2-paper-of-the-university-of-oxford/2019-resit/5/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/6/a/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability-resit/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/digital-systems-linear-algebra-introduction-to-formal-proof/1/f/solution.md)
- [C](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2024/paper-3/7/c.md)
- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2024/paper-3/7/h/solution.md)
- [RC low-pass laboratory](rc-low-pass-laboratory.md)
- [Square wave](square-wave.md)
- [Square-wave response of an RC low-pass filter](square-wave-response-of-an-rc-low-pass-filter.md)

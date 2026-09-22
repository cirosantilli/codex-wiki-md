<h1 id="fejer-first-moment-approximation-bound">Fejér first-moment approximation bound</h1>

↑ **Parent:** [Fejér sum](fejer-sum.md)

The normalized [Fejér kernel](fejer-kernel.md) satisfies $0\le F_n(t)\le\min\{n/(2\pi),\pi/(2nt^2)\}$ on $0<|t|\le\pi$. Splitting its first absolute moment at $1/n$ gives $\int|t|F_n(t)dt\le1/(2\pi n)+(\pi/n)\log(\pi n)$. The chaining inequality for the [modulus of continuity](modulus-of-continuity.md), $\omega(f,t)\le(1+t/\delta)\omega(f,\delta)$, then bounds the [Fejér sum](fejer-sum.md) error by $\omega(f,\delta)[1+\delta^{-1}\int|t|F_n]$. Taking $\delta=\log n/n$ proves the stated bound for $n\ge2$ and hence [uniform convergence](uniform-convergence.md) for continuous periodic functions. The logarithm vanishes at $n=1$, so the displayed estimate is not intended at that index.

**Table of contents**

- [Fractional-scale Fejér approximation bound](fractional-scale-fejer-approximation-bound.md)

## ↑ Ancestors (7)

1. [Fejér sum](fejer-sum.md)
2. [Fejér kernel](fejer-kernel.md)
3. [Fourier series](fourier-series-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/1/solution.md)

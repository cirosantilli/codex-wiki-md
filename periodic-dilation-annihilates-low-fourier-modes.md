# Periodic dilation annihilates low Fourier modes

↑ **Parent:** [Fourier coefficient](fourier-coefficient.md)

If $f$ is integrable and $2\pi$-periodic and $n$ is a positive integer, then $\int_0^{2\pi}f(nx)e^{imx}\,dx=0$ for every integer $m$ with $0<|m|<n$. Split the integral into $n$ equal intervals and substitute $y=nx-2\pi j$ to obtain

$$
\frac1n\int_0^{2\pi}f(y)e^{imy/n}\,dy
\sum_{j=0}^{n-1}e^{2\pi imj/n}=0.
$$

The [root of unity](root-of-unity.md) sum vanishes by the finite [geometric series](geometric-series.md) formula. The zero mode is $\int f$, so a mean-zero dilated function is orthogonal to all [trigonometric polynomials](trigonometric-polynomial.md) of degree at most $n-1$.

## ↑ Ancestors (6)

1. [Fourier coefficient](fourier-coefficient.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/3/b/solution.md)

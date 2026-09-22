# Periodic distribution

↑ **Parent:** [Distribution (mathematical analysis)](distribution-mathematical-analysis.md)

A [distribution](distribution-mathematical-analysis.md) has period $T>0$ if the displayed equality holds for every [test function](test-function.md) $\phi$. This agrees with $f(x+T)=f(x)$ [almost everywhere](almost-everywhere.md) for a [regular distribution](regular-distribution.md). If $u$ is a [tempered distribution](tempered-distribution.md), density of [test functions](test-function.md) in the [Schwartz space](schwartz-space.md) extends the identity to all [Schwartz functions](schwartz-function.md).

For a [test function](test-function.md) $\Psi$ with $\sum_k\Psi(x+kT)=1$, one has

$$
\langle u,\phi\rangle=\left\langle u,\Psi(x)\sum_k\phi(x+kT)\right\rangle.
$$

Indeed, expand $\phi=\sum_k\Psi(x+kT)\phi(x)$ in the [Schwartz space](schwartz-space.md) and move each translation to $\phi$ by periodicity. All [Schwartz seminorms](schwartz-seminorm.md) of the localized terms decay faster than any power of $|k|$, justifying the sum of pairings. This localization permits rigorous [Fourier coefficients](fourier-coefficient.md) without multiplying a [distribution](distribution-mathematical-analysis.md) by a discontinuous window.

## ↑ Ancestors (6)

1. [Distribution (mathematical analysis)](distribution-mathematical-analysis.md)
2. [Distribution theory](distribution-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fourier transform of a periodic distribution](fourier-transform-of-a-periodic-distribution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/3/a/ii/solution.md)
- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/3/a/iv/solution.md)

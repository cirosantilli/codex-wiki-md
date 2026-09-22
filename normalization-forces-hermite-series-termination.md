# Normalization forces Hermite-series termination

↑ **Parent:** [Power series solutions of the Hermite differential equation](power-series-solutions-of-the-hermite-differential-equation.md)

For the [Hermite differential equation](hermite-differential-equation.md) $f''-2\xi f'+(\epsilon-1)f=0$ with real $\epsilon$, the [wavefunction](wave-function-split.md) $e^{-\xi^2/2}f$ is square integrable on the real line only if $f$ is a [polynomial](polynomial-split.md). To prove this without assuming that even and odd tails cannot cancel, project a square-integrable solution onto its even and odd parts first. Each projection remains square integrable and satisfies the same equation.

In either nonterminating parity sequence, $b_j=a_{2j+p}$ obeys

$$
\frac{b_{j+1}}{b_j}=\frac{4j+2p+1-\epsilon}{(2j+p+2)(2j+p+1)}\sim\frac1j.
$$

The tail has constant complex phase. For any fixed $0<\delta<1/2$, comparison with $(1-\delta)/(j+1)$ bounds its coefficient magnitudes below by $K(1-\delta)^j/j!$ for sufficiently large $j$. Thus on the positive real axis the tail dominates a positive multiple of $\xi^p e^{(1-\delta)\xi^2}$ after subtraction of finitely many terms. The [Gaussian function](gaussian-function.md) factor leaves exponential growth $e^{(1/2-\delta)\xi^2}$, contradicting the [square-integrable](square-integrable-function.md) condition. Hence each nonzero parity sequence terminates. Its top coefficient forces $\epsilon=2n+1$, giving [Hermite oscillator quantization](hermite-oscillator-quantization.md) and a [Hermite polynomial](hermite-polynomial.md) of degree $n$.

## ↑ Ancestors (6)

1. [Power series solutions of the Hermite differential equation](power-series-solutions-of-the-hermite-differential-equation.md)
2. [Hermite differential equation](hermite-differential-equation.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-quantum-theory-course-of-the-university-of-oxford/2014/2/c/solution.md)

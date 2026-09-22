# Fourier stability threshold for a mixed-width heat scheme

↑ **Parent:** [Semidiscrete Fourier transform](semidiscrete-fourier-transform.md)

Consider an implicit centered heat stencil of width $\Delta x$ weighted by $\theta$, combined with an explicit centered stencil of width $2\Delta x$ weighted by $1-\theta$. With $\mu=\kappa\Delta t/(\Delta x)^2$, its [amplification factor](amplification-factor.md) is $G(\xi)=[1-\mu(1-\theta)\sin^2\xi]/[1+4\mu\theta\sin^2(\xi/2)]$. For $0\leq\theta<1/2$, contraction in the discrete $\ell^2$ norm holds exactly under the displayed condition. It is unconditional for $1/2\leq\theta\leq1$. Put $v=\sin^2(\xi/2)$: the condition $G\geq-1$ reduces to $4\mu v[(1-2\theta)-(1-\theta)v]\leq2$. Maximizing this concave quadratic proves the threshold; the [Parseval identity](parseval-identity.md) converts the multiplier bound into contraction.

## ↑ Ancestors (6)

1. [Semidiscrete Fourier transform](semidiscrete-fourier-transform.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/a/2/b/solution.md)

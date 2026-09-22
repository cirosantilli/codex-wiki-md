# Fourier sine series of a squared sine

↑ **Parent:** [Fourier sine series](fourier-sine-series.md)

On $0\leq x\leq L$, the [Fourier sine series](fourier-sine-series.md) of $\sin^2(\pi x/L)$ has zero even-index coefficients and odd-index coefficients $b_n=8/[\pi n(4-n^2)]$. Substitute $u=\pi x/L$ in the coefficient integral and use $\sin^2u\sin(nu)=\tfrac12\sin(nu)-\tfrac14\sin((n+2)u)-\tfrac14\sin((n-2)u)$. For odd $n$, integrating gives $b_n=(2/\pi)[1/n-\tfrac12(1/(n+2)+1/(n-2))]$; reflection about the midpoint makes the even coefficients zero. The $O(n^{-3})$ decay gives absolute and uniform convergence, and [Fourier orthogonality](fourier-orthogonality.md) identifies the sum. In the [heat equation](heat-equation.md) with zero endpoint temperatures, multiply each coefficient by $\exp[-\kappa(n\pi/L)^2t]$. With insulated endpoints, the same initial profile is instead just the constant and second cosine modes of a [Fourier cosine series](fourier-cosine-series.md).

## ↑ Ancestors (6)

1. [Fourier sine series](fourier-sine-series.md)
2. [Fourier series](fourier-series-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2/20/b/solution.md)

# Generating function of the physicists' Hermite polynomials

↑ **Parent:** [Hermite polynomial](hermite-polynomial.md)

For the [Hermite polynomials](hermite-polynomial.md) in the Rodrigues normalization $H_n=(-1)^ne^{t^2}D^ne^{-t^2}$, differentiating gives $H_{n+1}=2tH_n-H_n'$ with $H_0=1$. Induction gives

$$
H_n(t)=n!\sum_{j=0}^{\lfloor n/2\rfloor}\frac{(-1)^j2^{n-2j}t^{n-2j}}{j!(n-2j)!}.
$$

Insert this into the exponential generating [series](series-mathematics.md) and reindex $n=m+2j$. The result factors into $\sum_m(2tz)^m/m!$ times $\sum_j(-z^2)^j/j!$, proving the displayed identity. Equivalently Taylor expansion of $e^{-(t-z)^2}$ in $z$ gives the same formula. This [generating function](generating-function.md) keeps the normalization distinct from the [Probabilists' Hermite polynomial](probabilists-hermite-polynomial.md) convention.

**Table of contents**

- [Generating-function proof of Hermite orthogonality](generating-function-proof-of-hermite-orthogonality.md)

## ↑ Ancestors (7)

1. [Hermite polynomial](hermite-polynomial.md)
2. [Orthogonal polynomial](orthogonal-polynomial-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Generating-function proof of Hermite orthogonality](generating-function-proof-of-hermite-orthogonality.md)

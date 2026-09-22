# Generating-function proof of Hermite orthogonality

↑ **Parent:** [Generating function of the physicists' Hermite polynomials](generating-function-of-the-physicists-hermite-polynomials.md)

Multiply two copies of the [generating function of the physicists' Hermite polynomials](generating-function-of-the-physicists-hermite-polynomials.md) and integrate against $e^{-t^2}$. Completing the square gives

$$
\int_{\mathbb R}e^{-t^2}e^{2ty-y^2}e^{2tz-z^2}dt=\sqrt\pi e^{2yz}.
$$

Comparing coefficients gives the displayed [orthogonality](orthogonal-vectors.md) and normalization. Equivalently differentiation in $y,z$ at zero justifies coefficient extraction by the Gaussian integrable bound on compact parameter ranges. Hence the unnormalized [Hermite functions](hermite-function.md) $e^{-t^2/2}H_n(t)$ have [norm](norm.md) $\pi^{1/4}\sqrt{2^nn!}$. This proves their mutual [orthogonality](orthogonal-vectors.md); [completeness](completeness.md) of that family is an additional assertion.

## ↑ Ancestors (8)

1. [Generating function of the physicists' Hermite polynomials](generating-function-of-the-physicists-hermite-polynomials.md)
2. [Hermite polynomial](hermite-polynomial.md)
3. [Orthogonal polynomial](orthogonal-polynomial-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

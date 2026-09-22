# Legendre polynomial evaluation representer

↑ **Parent:** [Legendre polynomial](legendre-polynomial.md)

For [orthonormal](orthonormal-set.md) [Legendre polynomials](legendre-polynomial.md) on $[-1,1]$, the [polynomial](polynomial-split.md) $q_n$ represents evaluation at zero on polynomials of degree at most $n$: $\langle r,q_n\rangle=r(0)$. This follows by expanding $r$ in the [orthonormal basis](orthonormal-basis.md), or from the [Riesz representation theorem](riesz-representation-theorem.md). With $M=\lfloor n/2\rfloor$ and $c_m=\binom{2m}{m}/4^m$, orthonormality gives

$$
\|q_n\|_2^2=\frac12\sum_{m=0}^M(4m+1)c_m^2=\frac{(2M+1)^2c_M^2}{2}.
$$

The last identity telescopes using $c_m/c_{m-1}=(2m-1)/(2m)$. The norms are unbounded: $c_m\geq1/(2m+1)$ makes the sum dominate a divergent [harmonic series](harmonic-series.md). Thus the evaluation identities hold eventually for every fixed [polynomial](polynomial-split.md) but cannot extend to convergence for every $L^2$ vector, by the [Uniform boundedness principle](uniform-boundedness-principle.md). Point evaluation is also not defined on $L^2$ equivalence classes.

## ↑ Ancestors (10)

1. [Legendre polynomial](legendre-polynomial.md)
2. [Legendre differential equation](legendre-differential-equation.md)
3. [Second-order linear differential equation](second-order-linear-differential-equation.md)
4. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
5. [Ordinary differential equation](ordinary-differential-equation.md)
6. [Differential equation](differential-equation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

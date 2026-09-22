# Poisson potential of an exponential-over-radius source

↑ **Parent:** [Poisson's equation](poisson-s-equation.md)

For $\beta>0$, solve $\nabla^2\phi=-\rho$ in three dimensions with $\rho(r)=Ae^{-\beta r}/r$, finite potential at the origin and decay at infinity. The [Green function](green-s-function-split.md) is $1/(4\pi|\mathbf r-\mathbf r'|)$ in this sign convention. The angular integral supplied by the [spherical shell theorem](spherical-shell-theorem.md) gives

$$
\phi(r)=\frac1r\int_0^r s^2\rho(s)\,ds+\int_r^\infty s\rho(s)\,ds
=\boxed{\frac{A(1-e^{-\beta r})}{\beta^2r}}.
$$

The value at the origin is the limit $A/\beta$. A second derivation sets $u=r\phi$: the radial [Poisson equation](poisson-s-equation.md) becomes $u''=-Ae^{-\beta r}$. Decay excludes the constant-potential term and boundedness at the origin cancels the remaining $1/r$ singularity. Although the source is locally [integrable](integrability.md), it is singular at the origin; the resulting potential solves the equation there in the sense of [distributions](distribution-mathematical-analysis.md), without an extra [Dirac delta](dirac-delta-function.md).

## ↑ Ancestors (6)

1. [Poisson's equation](poisson-s-equation.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/3/b/iii/solution.md)

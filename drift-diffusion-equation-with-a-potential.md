# Drift-diffusion equation with a potential

↑ **Parent:** [Diffusion equation](diffusion-equation-split.md)

For positive [diffusivity](diffusion-coefficient.md) $D(x)$, a [diffusion equation](diffusion-equation-split.md) with potential-driven drift has [diffusive flux](diffusive-flux.md) $J=-D(c_x+\beta V'c)$. On a finite interval with zero [flux](flux.md) at both endpoints, the total amount is conserved. The substitution $c=e^{-\lambda t}e^{-\beta V}y$ converts the decay [eigenvalue problem](eigenvalue-problem.md) to the [Sturm-Liouville problem](sturm-liouville-problem.md)

$$
-(py')'=\lambda wy,\qquad p=De^{-\beta V},\quad w=e^{-\beta V},\quad py'=0\text{ at the endpoints}.
$$

The [Rayleigh quotient](rayleigh-quotient.md) is $\lambda=\int p|y'|^2/\int w|y|^2\geq0$. Its zero [eigenfunction](eigenfunction.md) is constant, giving the [stationary solution](stationary-solution.md) $c_{\rm eq}=C e^{-\beta V}$. This is a spatial [Boltzmann distribution](boltzmann-distribution.md); $D$ changes relaxation rates but cancels out of the zero-[flux](flux.md) equilibrium profile. For a sufficiently regular positive $D$ and bounded $V$, the constant eigenfunction is the unique zero mode up to scale.

## ↑ Ancestors (6)

1. [Diffusion equation](diffusion-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/1/a/solution.md)

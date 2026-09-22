# Compressed Euler-Bernoulli beam and its endpoint-dependent buckling threshold

↑ **Parent:** [Euler-Bernoulli beam equation](euler-bernoulli-beam-equation.md)

Positive compression $\alpha$ contributes negative quadratic [potential energy](potential-energy.md) $-\alpha\phi_x^2/2$, while positive [bending stiffness](bending-stiffness.md) $\beta$ contributes $\beta\phi_{xx}^2/2$. A [plane wave](plane-wave.md) has $\omega^2=(\beta k^4-\alpha k^2)/\rho$, so sufficiently long waves grow exponentially. For displacement-fixed, moment-free endpoints at $0,l$, the [natural boundary conditions for a free endpoint](natural-boundary-conditions-for-a-free-endpoint.md) on the slope give $\phi_{xx}=0$ as well as $\phi=0$. The modes are $\sin(n\pi x/l)$, and the first [Euler buckling of an elastic filament](euler-buckling-of-an-elastic-filament.md) threshold is $\alpha_c=\beta\pi^2/l^2$. For truly clamped ends, $\phi=\phi_x=0$, the threshold is instead $4\pi^2\beta/l^2$, with first static mode $1-\cos(2\pi x/l)$. More generally,

$$
\alpha_c=\beta\inf_{\phi\ne0}\frac{\int_0^l\phi_{xx}^2dx}{\int_0^l\phi_x^2dx},
$$

with the infimum taken over the specified endpoint class. At threshold there is a static zero mode and a marginal linear-in-time partner in the linear dynamics; above it the straight configuration is unstable.

## ↑ Ancestors (7)

1. [Euler-Bernoulli beam equation](euler-bernoulli-beam-equation.md)
2. [Linear elasticity](linear-elasticity.md)
3. [Elasticity (physics)](elasticity-physics-split.md)
4. [Continuum mechanics](continuum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2022/2/e/solution.md)

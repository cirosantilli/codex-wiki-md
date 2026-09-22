<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widehat{\mathbf u}$ and $\widehat p$ be the complex [plane wave](../../../../plane-wave.md) amplitudes and set $k_x=k_\perp$, $k_z=k_\parallel$. The [linearized Euler equations](../../../../linearized-euler-equations.md) in the rotating frame are

$$
\begin{aligned}
-i\omega\widehat u_x&=-ik_\perp\widehat p+2\Omega\widehat u_y,\\
-i\omega\widehat u_y&=-2\Omega\widehat u_x,\\
-i\omega\widehat u_z&=-ik_\parallel\widehat p,\\
k_\perp\widehat u_x+k_\parallel\widehat u_z&=0.
\end{aligned}
$$

Here $p$ is [pressure](../../../../pressure-split.md) per unit [mass density](../../../../density.md), including the centrifugal potential. The last line is [incompressibility](../../../../incompressible-flow.md), not an additional equation of state.

Taking the [curl](../../../../curl.md) eliminates [pressure](../../../../pressure-split.md). For constant $\boldsymbol\Omega$ and a [divergence-free vector field](../../../../divergence-free-vector-field.md), $\nabla\times(2\mathbf u\times\boldsymbol\Omega)=2(\boldsymbol\Omega\cdot\nabla)\mathbf u$. Thus the [inertial-wave vorticity equation](../../../../inertial-wave-vorticity-equation.md) gives

$$
-i\omega(i\mathbf k\times\widehat{\mathbf u})
=2i\Omega k_\parallel\widehat{\mathbf u},\qquad
\omega\mathbf k\times\widehat{\mathbf u}=2i\Omega k_\parallel\widehat{\mathbf u}.
$$

Apply $\mathbf k\times$ once more and use $\mathbf k\times(\mathbf k\times\widehat{\mathbf u})=-k^2\widehat{\mathbf u}$. For a nonzero oscillatory amplitude,

$$
-\omega k^2\widehat{\mathbf u}
=2i\Omega k_\parallel\frac{2i\Omega k_\parallel}{\omega}\widehat{\mathbf u},
$$

so the [inertial-wave dispersion relation](../../../../inertial-wave-dispersion-relation.md) is

$$
\boxed{\omega^2=4\Omega^2\frac{k_\parallel^2}{k^2},\qquad
\omega_\sigma=\sigma\,2\Omega\frac{k_\parallel}{k},\quad\sigma=\pm1.}
$$

The restoring influence is the [Coriolis acceleration](../../../../coriolis-acceleration.md). In particular $|\omega|\le2|\Omega|$. For $k_\parallel=0$, the projected linear dynamics have zero [frequency](../../../../frequency.md); these are steady balanced disturbances rather than the nonzero-frequency branch used in the division above. The spatially uniform $k=0$ mode must be treated separately from this [dispersion relation](../../../../dispersion-relation-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

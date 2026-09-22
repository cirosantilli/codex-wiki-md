<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Eliminating the [shear stress](../../../../../shear-stress.md) from the two linear equations gives the [Maxwell shear-wave dispersion](../../../../../maxwell-shear-wave-dispersion.md) equation in physical space,

$$
\tau\partial_t^2u+\partial_tu=\nu\partial_y^2u,
\qquad \nu=\frac{\mu}{\rho_0},
$$

where $\nu$ is the [kinematic viscosity](../../../../../kinematic-viscosity.md). Substitution of a [Fourier mode](../../../../../fourier-mode.md) $e^{iky+\sigma t}$ gives

$$
\tau\sigma^2+\sigma+\nu k^2=0,
\qquad
\boxed{\sigma_\pm=\frac{-1\pm\sqrt{1-4\tau\nu k^2}}{2\tau}.}
$$

These are temporal exponents: the oscillation [angular frequency](../../../../../angular-frequency.md) is the imaginary part of $\sigma$, with the sign determined by the selected time convention. For $4\tau\nu k^2<1$ both exponents are real and nonpositive. At equality the repeated exponent is $-1/(2\tau)$; generic solutions include $t e^{-t/(2\tau)}$. Above the threshold the modes are damped propagating shear disturbances:

$$
\sigma_\pm=-\frac1{2\tau}\pm i\sqrt{\frac{\nu k^2}{\tau}-\frac1{4\tau^2}}.
$$

At large $|k|$ their [phase velocity](../../../../../phase-velocity.md) tends to $\sqrt{\nu/\tau}=\sqrt{G_{\rm el}/\rho_0}$.

For the limit $\tau\to0$ at fixed $\mu,\rho_0$ and $k$, expansion of the [square root](../../../../../square-root.md) gives

$$
\boxed{\sigma_{\rm slow}=-\nu k^2+O(\tau),\qquad \sigma_{\rm fast}=-\frac1\tau+\nu k^2+O(\tau).}
$$

After a short initial relaxation, the surviving branch obeys the [diffusion equation](../../../../../diffusion-equation-split.md) $u_t=\nu u_{yy}$ of a [Newtonian fluid](../../../../../newtonian-fluid.md). The fast branch disappears on the vanishing [viscoelastic relaxation time](../../../../../viscoelastic-relaxation-time.md); at $k=0$ the two exponents are exactly $0$ and $-1/\tau$. This limit is not uniform in $k$: modes with $k$ of order $(\tau\nu)^{-1/2}$ still sample the oscillatory transition. If instead $G_{\rm el}=\mu/\tau$ is held fixed as $\tau\to0$, then $\mu\to0$ and the fixed-$k$ slow exponent tends to zero. The ordinary [Newtonian fluid](../../../../../newtonian-fluid.md) limit therefore specifies which material parameter is held fixed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2016](../../../../2016-split.md)
5. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../../split.md)
6. [Advanced fluid dynamics course of the University of Oxford](../../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

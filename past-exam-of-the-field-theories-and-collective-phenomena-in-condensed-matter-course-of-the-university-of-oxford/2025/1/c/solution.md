<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $x=x_0+y$, so the fluctuation has homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) $y(0)=y(T_E)=0$. Because $\dot x_0$ is constant, the cross term in the [Euclidean action](../../../../euclidean-action.md) vanishes exactly:

$$
m\int_0^{T_E}\dot x_0\dot y\,d\tau
=m\dot x_0[y(T_E)-y(0)]=0.
$$

Consequently

$$
S_{\mathrm{Euc}}[x_0+y]
=\frac{m(x_f-x_i)^2}{2T_E}+\frac m2\int_0^{T_E}\dot y^2d\tau.
$$

Translation of each intermediate integration variable has [Jacobian determinant](../../../../jacobian-determinant.md) one in the [time-sliced configuration-space path integral](../../../../time-sliced-configuration-space-path-integral.md). This is an exact [classical-path factorization of a quadratic path integral](../../../../classical-path-factorization-of-a-quadratic-path-integral.md), giving

$$
\boxed{\langle x_f|e^{-\beta H}|x_i\rangle
=\mathcal N\exp\!\left[-\frac{m(x_f-x_i)^2}{2\beta\hbar^2}\right],
\quad
\mathcal N=\int_{y(0)=0}^{y(\beta\hbar)=0}\mathcal D y\,
\exp\!\left[-\frac{m}{2\hbar}\int_0^{\beta\hbar}\dot y^2d\tau\right].}
$$

The fluctuation [Euclidean action](../../../../euclidean-action.md), the homogeneous [boundary conditions](../../../../boundary-condition.md), and the measure normalization contain neither $x_i$ nor $x_f$. Hence **$\mathcal N$ is independent of both endpoint [positions](../../../../position.md)**. It depends on $\beta,m,\hbar$.

With the standard position-state normalization, the [Euclidean free-particle bridge amplitude](../../../../euclidean-free-particle-bridge-amplitude.md) is

$$
\boxed{\mathcal N=\sqrt{\frac{m}{2\pi\beta\hbar^2}}.}
$$

For example, a [momentum](../../../../momentum-split.md) resolution gives a one-dimensional [Gaussian integral](../../../../gaussian-integral.md),

$$
\langle x_f|e^{-\beta H}|x_i\rangle
=\int_{-\infty}^{\infty}\frac{dp}{2\pi\hbar}
\exp\!\left[-\frac{\beta p^2}{2m}+\frac{ip(x_f-x_i)}{\hbar}\right],
$$

whose evaluation gives the same exponent and prefactor. In particular, the result integrates to one over $x_f$ at fixed $x_i$, as required for its [heat kernel](../../../../heat-kernel.md) interpretation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the field theories and collective phenomena in condensed matter course of the University of Oxford](../../../split.md)
5. [Field theories and collective phenomena in condensed matter course of the University of Oxford](../../../../field-theories-and-collective-phenomena-in-condensed-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

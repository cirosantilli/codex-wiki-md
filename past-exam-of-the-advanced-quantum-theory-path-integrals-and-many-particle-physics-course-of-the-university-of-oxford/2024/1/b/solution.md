<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

After the shift $x(\tau)=x_0(\tau)+y(\tau)$, the endpoint values of $y$ are both zero. Expanding the [Euclidean action](../../../../euclidean-action.md) gives

$$
S[x_0+y]=S[x_0]+S[y]
+m\int_0^{\mathcal T}(\dot x_0\dot y+\omega^2x_0y)\,d\tau.
$$

By [integration by parts](../../../../integration-by-parts.md), the cross term is

$$
m[\dot x_0y]_0^{\mathcal T}
+m\int_0^{\mathcal T}(-\ddot x_0+\omega^2x_0)y\,d\tau=0.
$$

The first term vanishes by the homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), and the second by the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md). The translation has unit [Jacobian determinant](../../../../jacobian-determinant.md) in the [time-sliced configuration-space path integral](../../../../time-sliced-configuration-space-path-integral.md), so $\mathcal D x=\mathcal D y$. Consequently [classical-path factorization of a quadratic path integral](../../../../classical-path-factorization-of-a-quadratic-path-integral.md) is exact here:

$$
\boxed{\langle x|e^{-\beta H}|x\rangle=e^{-S[x_0]/\hbar}Z,\qquad
Z=\int_{y(0)=y(\mathcal T)=0}\mathcal D y\,
\exp\!\left[-\frac m{2\hbar}\int_0^{\mathcal T}(\dot y^2+\omega^2y^2)\,d\tau\right].}
$$

All dependence on the common endpoint $x$ lies in

$$
\boxed{e^{-S[x_0]/\hbar}
=\exp\!\left[-\frac{m\omega x^2}{\hbar}\tanh\!\left(\frac{\beta\hbar\omega}{2}\right)\right],
\qquad Z\text{ is independent of }x.}
$$

The endpoint domain and the integrand defining $Z$ are the same for every $x$. This $Z$ is a zero-endpoint [Gaussian path integral](../../../../gaussian-path-integral.md); the [canonical partition function](../../../../canonical-partition-function.md) instead integrates the entire diagonal kernel over $x$. The final sentence of the printed part omits $/\hbar$ from its exponential: the physical [Boltzmann factor](../../../../boltzmann-factor.md) has the dimensionless exponent $-S/\hbar$.

An optional normalization check uses the [Dirichlet oscillator fluctuation determinant](../../../../dirichlet-oscillator-fluctuation-determinant.md). Its [eigenvalues](../../../../eigenvalue.md) are $m[(n\pi/\mathcal T)^2+\omega^2]$, $n\ge1$. Relative to the free-particle [Gaussian path integral](../../../../gaussian-path-integral.md), the [hyperbolic-sine infinite product](../../../../hyperbolic-sine-infinite-product.md) gives

$$
\frac{Z}{\sqrt{m/(2\pi\hbar\mathcal T)}}
=\prod_{n=1}^{\infty}\left[1+\frac{\omega^2\mathcal T^2}{n^2\pi^2}\right]^{-1/2}
=\sqrt{\frac{\omega\mathcal T}{\sinh(\omega\mathcal T)}}.
$$

Thus $Z=\sqrt{m\omega/[2\pi\hbar\sinh(\beta\hbar\omega)]}$. Integrating the resulting [diagonal thermal kernel of a quantum harmonic oscillator](../../../../diagonal-thermal-kernel-of-a-quantum-harmonic-oscillator.md) by a [Gaussian integral](../../../../gaussian-integral.md) yields $\operatorname{Tr}e^{-\beta H}=[2\sinh(\beta\hbar\omega/2)]^{-1}$, including the [zero-point energy](../../../../zero-point-energy.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

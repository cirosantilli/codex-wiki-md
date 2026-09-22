<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Make the [Wick rotation](../../../../wick-rotation.md) $t'=-i\tau$, and write $T_E=\beta\hbar$ for the final [imaginary time](../../../../imaginary-time.md), where $\beta$ is [inverse temperature](../../../../inverse-temperature.md) and $\hbar$ is the [reduced Planck constant](../../../../reduced-planck-constant.md). Then $dt'=-i\,d\tau$ and $dx/dt'=i\,dx/d\tau$. Thus the continued [action](../../../../action.md) is

$$
S=i\int_0^{T_E}\left[\frac m2\left(\frac{dx}{d\tau}\right)^2+V(x)\right]d\tau
=iS_{\mathrm{Euc}},
\qquad
\boxed{S_{\mathrm{Euc}}[x]=\int_0^{\beta\hbar}\left[\frac m2\dot x^2+V(x)\right]d\tau.}
$$

Both the [kinetic energy](../../../../kinetic-energy.md) and the [potential energy](../../../../potential-energy.md) enter this [Euclidean action](../../../../euclidean-action.md) with positive signs relative to their real-time definitions. Also $e^{-iH(-i\beta\hbar)/\hbar}=e^{-\beta H}$, so the [Euclidean path integral](../../../../euclidean-path-integral.md) is

$$
\boxed{\langle x_f|e^{-\beta H}|x_i\rangle
=\int_{x(0)=x_i}^{x(T_E)=x_f}\mathcal D x\,
 e^{-S_{\mathrm{Euc}}[x]/\hbar}.}
$$

Its [boundary conditions](../../../../boundary-condition.md) fix the two endpoint [positions](../../../../position.md). They need not coincide: identifying and integrating over them would instead give the [thermal trace](../../../../thermal-trace.md).

The normalization of $\mathcal D x$ can be fixed without continuing a formal measure. Apply the [Trotter product formula](../../../../lie-product-formula.md) to $H=\hat p^2/(2m)+V(\hat x)$, divide $T_E$ into $M$ intervals of size $\epsilon=T_E/M$, and integrate the intermediate [positions](../../../../position.md). The resulting [time-sliced configuration-space path integral](../../../../time-sliced-configuration-space-path-integral.md) is

$$
\lim_{M\to\infty}
\left(\frac{m}{2\pi\hbar\epsilon}\right)^{M/2}
\int_{\mathbb R^{M-1}}\prod_{j=1}^{M-1}dx_j\,
\exp\!\left[-\frac1\hbar\sum_{j=1}^M
\left\{\frac{m(x_j-x_{j-1})^2}{2\epsilon}+\epsilon V(x_{j-1})\right\}\right],
\quad x_0=x_i,\quad x_M=x_f.
$$

This also explains the upper limit $\beta\hbar$ rather than $\beta$ when the [reduced Planck constant](../../../../reduced-planck-constant.md) has not been set to one.

## ↑ Ancestors (12)

1. [A](../a.md)
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

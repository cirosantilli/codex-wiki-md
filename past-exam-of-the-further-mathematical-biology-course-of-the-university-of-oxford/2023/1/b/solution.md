<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unit integrals of the profiles make $N_i(t)=\int_0^\infty n_i(\tau,t)\,d\tau$ the phase populations, and $f_i$ their normalized [cell-cycle age densities](../../../../cell-cycle-age-density.md). Assume the age tails vanish and the following integrals are finite. For a fixed profile define its mean exit [hazard function](../../../../hazard-function.md) by

$$
\boxed{\Lambda_i=\int_0^\infty\Gamma_i(\tau)f_i(\tau)\,d\tau,\qquad i=1,2.}
$$

These constants have units of inverse time. Integrating the [age-structured population equations](../../../../age-structured-population-equation.md) and using the [boundary conditions](../../../../boundary-condition.md) gives

$$
\begin{aligned}
N_1'&=-[n_1(\tau,t)]_0^\infty-\int_0^\infty\Gamma_1n_1\,d\tau
=n_1(0,t)-\Lambda_1N_1,\\
N_2'&=-[n_2(\tau,t)]_0^\infty-\int_0^\infty\Gamma_2n_2\,d\tau
=n_2(0,t)-\Lambda_2N_2.
\end{aligned}
$$

The incoming [fluxes](../../../../flux.md) are $n_1(0,t)=2\Lambda_2N_2$ and $n_2(0,t)=\Lambda_1N_1$, so

$$
\boxed{\frac{d}{dt}\begin{pmatrix}N_1\\N_2\end{pmatrix}
=\begin{pmatrix}-\Lambda_1&2\Lambda_2\\\Lambda_1&-\Lambda_2\end{pmatrix}
\begin{pmatrix}N_1\\N_2\end{pmatrix}.}
$$

The [separable-profile closure for an age-structured population](../../../../separable-profile-closure-for-an-age-structured-population.md) has a qualification: arbitrary age-dependent [hazard functions](../../../../hazard-function.md) do not give this constant-coefficient [ordinary differential equation](../../../../ordinary-differential-equation.md) for arbitrary [initial conditions](../../../../initial-condition.md). Without fixed $f_i$, the effective exit rates are $\int\Gamma_i n_i\,d\tau/N_i$ and can vary with time. Moreover, an exact positive [separation of variables](../../../../separation-of-variables.md) with both profiles fixed forces $N_2/N_1$ to be constant through the incoming [fluxes](../../../../flux.md), hence selects a common exponential mode. The displayed [ordinary differential equation](../../../../ordinary-differential-equation.md) is the necessary integrated system for such profiles; it is also exact for arbitrary populations when both [hazard functions](../../../../hazard-function.md) are age independent.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

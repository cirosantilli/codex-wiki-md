<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A [passive scalar](../../../../../../passive-scalar.md) $\theta$ is transported by the [velocity field](../../../../../../velocity-field.md) without feeding back on it:

$$
\partial_t\theta+\mathbf u\cdot\nabla\theta=\kappa\Delta\theta.
$$

Take its mean to be zero, and define the [scalar dissipation rate](../../../../../../scalar-dissipation-rate.md) by the half-[scalar variance](../../../../../../scalar-variance.md) convention $\chi=\kappa\langle|\nabla\theta|^2\rangle$. In a statistically equilibrated [energy cascade](../../../../../../energy-cascade.md) of scalar fluctuations, this is also the flux of half-[scalar variance](../../../../../../scalar-variance.md) toward small scales.

The [Kolmogorov two-thirds law](../../../../../../kolmogorov-two-thirds-law.md) gives a typical [velocity increment](../../../../../../velocity-increment.md) $\delta u_r\sim(\epsilon r)^{1/3}$ and hence [eddy turnover time](../../../../../../eddy-turnover-time.md) $\tau_r\sim r/\delta u_r\sim\epsilon^{-1/3}r^{2/3}$. Assuming local scalar transfer on this same time scale, $\chi\sim\langle(\Delta\theta)^2\rangle/\tau_r$. The [Obukhov-Corrsin theory](../../../../../../obukhov-corrsin-theory.md) therefore gives the scalar analogue:

$$
\boxed{\langle(\Delta\theta)^2\rangle=C_\theta\chi\epsilon^{-1/3}r^{2/3}}.
$$

This applies to separations at which both direct forcing and molecular [diffusion](../../../../../../diffusion.md) are negligible and the transporting [velocity increments](../../../../../../velocity-increment.md) lie in the [inertial range](../../../../../../inertial-range.md). For very large or very small ratios $\nu/\kappa$, the scalar and velocity cutoff scales differ, so this common range must be checked. Defining $\chi$ as dissipation of the full [scalar variance](../../../../../../scalar-variance.md) instead simply changes the convention for $C_\theta$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

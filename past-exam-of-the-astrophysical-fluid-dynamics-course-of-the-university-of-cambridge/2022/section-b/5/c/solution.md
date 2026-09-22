<h1 id="section-b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\nu>0$ and positive $\Psi$, set $f=\log\Psi$, so the [Cole-Hopf transformation](../../../../../cole-hopf-transformation.md) is $u=-2\nu f_x$. Substitution into the [viscous Burgers equation](../../../../../viscous-burgers-equation.md) gives

$$
u_t+uu_x-\nu u_{xx}
=-2\nu\partial_x\left(f_t-\nu f_{xx}-\nu f_x^2\right)
=-2\nu\partial_x\left(\frac{\Psi_t-\nu\Psi_{xx}}{\Psi}\right)=0.
$$

Hence the most general equation implied by this substitution is

$$
\Psi_t-\nu\Psi_{xx}=C(t)\Psi.
$$

The [time normalization in the Cole-Hopf transformation](../../../../../time-normalization-in-the-cole-hopf-transformation.md) accounts for the arbitrary function $C(t)$: multiplying $\Psi$ by a nonzero function of time leaves $\partial_x\log\Psi$ and therefore $u$ unchanged. Replacing $\Psi$ by $e^{-\int^tC(s)ds}\Psi$ sets $C=0$. With this conventional normalization,

$$
\boxed{\partial_t\Psi=\nu\partial_x^2\Psi,}
$$

the [heat equation](../../../../../heat-equation.md).

For each $j=1,2$, the function $\Psi_j=e^{\nu\kappa_j^2t+\kappa_jx}$ obeys $\partial_t\Psi_j=\nu\kappa_j^2\Psi_j=\nu\partial_x^2\Psi_j$. By the [superposition principle](../../../../../superposition-principle.md) for this linear [partial differential equation](../../../../../partial-differential-equation-split.md),

$$
\boxed{\Psi=e^{\nu\kappa_1^2t+\kappa_1x}+e^{\nu\kappa_2^2t+\kappa_2x}}
$$

is a solution, positive for all real $x,t,\kappa_1,\kappa_2$. Here $\kappa_j$ has units $\mathrm{m^{-1}}$ so both exponents are dimensionless. The positivity ensures that its logarithm and the resulting [velocity](../../../../../velocity.md) are regular.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

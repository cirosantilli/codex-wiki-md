<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [electric potential](../../../../../electric-potential.md) and [magnetic vector potential](../../../../../magnetic-vector-potential.md) represent the fields through $\mathbf B=\nabla\times\mathbf A$ and $\mathbf E=-\nabla\phi-\partial_t\mathbf A$. They are not unique: a differentiable function $\chi$ gives

$$
\boxed{\mathbf A\mapsto\mathbf A+\nabla\chi,\qquad
\phi\mapsto\phi-\partial_t\chi,}
$$

without changing either field. [Gauge fixing](../../../../../gauge-fixing.md) restricts this freedom to suit the sources, boundaries or symmetry; it does not alter observables.

The [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\nabla\cdot\mathbf A+c^{-2}\partial_t\phi=0$ is [Lorentz covariant](../../../../../lorentz-covariance.md). [Maxwell's equations](../../../../../maxwell-equations-split.md) then reduce to sourced [wave equations](../../../../../wave-equation-split.md),

$$
(\nabla^2-c^{-2}\partial_t^2)\phi=-\rho/\epsilon_0,\qquad
(\nabla^2-c^{-2}\partial_t^2)\mathbf A=-\mu_0\mathbf J.
$$

Retarded solutions implement causal radiation conditions. This gauge is useful for radiation and relativistic calculations; residual transformations obey the homogeneous [wave equation](../../../../../wave-equation-split.md).[§18–6, Eqs. (18.23)–(18.25): gauge choice and potential wave equations](../../../../../the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md)

The [Coulomb gauge](../../../../../coulomb-gauge.md) $\nabla\cdot\mathbf A=0$ instead gives $\nabla^2\phi=-\rho/\epsilon_0$. Its [electric potential](../../../../../electric-potential.md) is an instantaneous Poisson solution, but the accompanying [magnetic vector potential](../../../../../magnetic-vector-potential.md) makes the full physical [electric field](../../../../../electric-field-split.md) causal. It is useful in separating longitudinal [electric fields](../../../../../electric-field-split.md) from transverse radiation. In a source-free [vacuum](../../../../../vacuum.md) region, suitable radiation [boundary conditions](../../../../../boundary-condition.md) permit [radiation gauge](../../../../../radiation-gauge.md) $\phi=0$, $\nabla\cdot\mathbf A=0$, leaving two transverse plane-wave [polarizations](../../../../../polarization-waves.md). These extra conditions are not a gauge choice applicable unchanged to arbitrary nonzero charge distributions.

**Different gauges redistribute information between potentials; the same boundary-value problem gives the same [electric fields](../../../../../electric-field-split.md) and [magnetic fields](../../../../../magnetic-field-split.md).**

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

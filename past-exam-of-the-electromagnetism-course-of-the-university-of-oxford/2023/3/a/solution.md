<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With [charge density](../../../../charge-density.md) $\rho$, [current density](../../../../current-density.md) $\mathbf J$, and [speed of light](../../../../speed-of-light.md) $c=(\epsilon_0\mu_0)^{-1/2}$, the four [Maxwell equations](../../../../maxwell-equations-split.md) in [vacuum](../../../../vacuum.md) are

$$
\boxed{\begin{aligned}
\nabla\cdot\mathbf E&=\rho/\epsilon_0,&\nabla\cdot\mathbf B&=0,\\
\nabla\times\mathbf E&=-\partial_t\mathbf B,&
\nabla\times\mathbf B&=\mu_0\mathbf J+c^{-2}\partial_t\mathbf E.
\end{aligned}}
$$

The [electric potential](../../../../electric-potential.md) and [magnetic vector potential](../../../../magnetic-vector-potential.md) determine the [electric field](../../../../electric-field-split.md) and [magnetic field](../../../../magnetic-field-split.md) by

$$
\boxed{\mathbf E=-\nabla\phi-\partial_t\mathbf A,\qquad
\mathbf B=\nabla\times\mathbf A.}
$$

These definitions satisfy [Gauss's law for magnetism](../../../../gauss-s-law-for-magnetism.md) and [Faraday's law](../../../../faraday-s-law-of-induction.md) identically. The [Lorenz gauge condition](../../../../lorenz-gauge-condition.md) is

$$
\boxed{\nabla\cdot\mathbf A+c^{-2}\partial_t\phi=0.}
$$

Substituting into [Gauss's law](../../../../gauss-s-law.md) and using the [Lorenz gauge condition](../../../../lorenz-gauge-condition.md) gives

$$
\frac\rho{\epsilon_0}=-\nabla^2\phi-\partial_t(\nabla\cdot\mathbf A)
=-\nabla^2\phi+c^{-2}\partial_t^2\phi.
$$

For the [Ampère-Maxwell equation](../../../../ampere-s-circuital-law.md), the double-[curl](../../../../curl.md) identity gives

$$
\nabla(\nabla\cdot\mathbf A)-\nabla^2\mathbf A
=\mu_0\mathbf J-c^{-2}\nabla\partial_t\phi-c^{-2}\partial_t^2\mathbf A.
$$

The two [gradient](../../../../gradient.md) terms cancel by the [Lorenz gauge condition](../../../../lorenz-gauge-condition.md). Defining the [d'Alembert operator](../../../../d-alembert-operator.md) with the sign convention $\square=\nabla^2-c^{-2}\partial_t^2$, the remaining equations are

$$
\boxed{\square\phi=-\rho/\epsilon_0,\qquad
\square\mathbf A=-\mu_0\mathbf J.}
$$

Conversely, if the [electric potential](../../../../electric-potential.md) and [magnetic vector potential](../../../../magnetic-vector-potential.md) satisfy these [wave equations](../../../../wave-equation-split.md) and the [Lorenz gauge condition](../../../../lorenz-gauge-condition.md), the same substitutions in reverse give [Gauss's law](../../../../gauss-s-law.md) and the [Ampère-Maxwell equation](../../../../ampere-s-circuital-law.md). The other two [Maxwell equations](../../../../maxwell-equations-split.md) follow identically from the definitions, proving equivalence within the [Lorenz gauge](../../../../lorenz-gauge-condition.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the electromagnetism course of the University of Oxford](../../../split.md)
5. [Electromagnetism course of the University of Oxford](../../../../electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

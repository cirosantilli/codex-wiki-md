<h1 id="16b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the charge-generated [electric field](../../../../../../electric-field.md), use the [electric potential](../../../../../../electric-potential.md)

$$
\phi(\mathbf r,t)=\frac1{4\pi\varepsilon_0}\int\frac{\rho(\mathbf r',t)}{|\mathbf r-\mathbf r'|}\,dV',\qquad\mathbf E=-\nabla\phi.
$$

The [vector](../../../../../../vector.md) potential is time independent, so its usual additional contribution $-\partial_t\mathbf A$ is zero. The [continuity equation](../../../../../../continuity-equation.md) now gives

$$
\partial_t\mathbf E=-\frac1{4\pi\varepsilon_0}\nabla\int\frac{\dot\rho(\mathbf r',t)}s\,dV'=\frac1{4\pi\varepsilon_0}\nabla\int\frac{\nabla'\cdot\mathbf J(\mathbf r')}s\,dV'.
$$

Thus the second term in part (iii) is exactly the [displacement current](../../../../../../displacement-current.md) contribution $\mu_0\varepsilon_0\partial_t\mathbf E$, and

$$
\boxed{\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\varepsilon_0\partial_t\mathbf E.}
$$

This is the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md). The constructed field also has zero curl, consistent with the time-independent [magnetic field](../../../../../../magnetic-field.md) and [Faraday's law](../../../../../../faraday-s-law-of-induction.md). A static addition to the [electric field](../../../../../../electric-field.md) does not change this conclusion; the integral construction selects the fields sourced by the given densities rather than an independently added radiation field.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [16B](../../16b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

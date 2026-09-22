<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [divergence](../../../../divergence.md) of the [Ampère-Maxwell equation](../../../../ampere-s-circuital-law.md) and use that the [divergence of a curl is zero](../../../../divergence-of-a-curl-is-zero.md):

$$
0=\nabla\cdot(\nabla\times\mathbf B)
=\mu_0\nabla\cdot\mathbf J+\mu_0\epsilon_0\partial_t(\nabla\cdot\mathbf E)
=\mu_0(\nabla\cdot\mathbf J+\partial_t\rho).
$$

The last step uses [Gauss's law](../../../../gauss-s-law.md). Thus the [charge continuity equation](../../../../charge-continuity-equation.md) is exactly

$$
\boxed{J^\mu=(c\rho,\mathbf J),\qquad \partial_\mu J^\mu=\partial_t\rho+\nabla\cdot\mathbf J=0.}
$$

For a direct justification that this [four-current](../../../../four-current.md) is a [four-vector](../../../../four-vector.md), take one locally comoving population of [electric charges](../../../../electric-charge-split.md), with rest [charge density](../../../../charge-density.md) $\rho_0$ and [four-velocity](../../../../four-velocity.md) $U^\mu=\gamma(c,\mathbf v)$. Invariance of [electric charge](../../../../electric-charge-split.md) and [length contraction](../../../../length-contraction.md) give $\rho=\gamma\rho_0$ and $\mathbf J=\rho\mathbf v$, hence $J^\mu=\rho_0U^\mu$. Summing populations preserves the [four-vector](../../../../four-vector.md) rule. In particular, $c\rho'=\gamma(c\rho-\beta J_x)$ and $J'_x=\gamma(J_x-\beta c\rho)$. The [Lorentz invariance](../../../../lorentz-invariance.md) of its [four-divergence](../../../../four-divergence.md) then explains why [charge conservation](../../../../charge-conservation.md) holds in every [inertial frame](../../../../inertial-frame.md). A single zero-divergence condition alone would not determine a field's transformation law; the physical [charge density](../../../../charge-density.md) and [current density](../../../../current-density.md) provide the additional content.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

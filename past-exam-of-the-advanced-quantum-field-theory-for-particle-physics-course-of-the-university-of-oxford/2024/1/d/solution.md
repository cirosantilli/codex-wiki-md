<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Couple a nondynamical [background gauge field](../../../../background-gauge-field.md) $B_\mu$ to the [Dirac current](../../../../dirac-current.md), choosing a plus sign for the source term:

$$
\boxed{Z[B]=\mathcal N\int\mathcal D\bar\psi\,\mathcal D\psi\,
\exp\left\{i\int d^4x\,[\bar\psi(i\not\partial-m)\psi+B_\mu\bar\psi\gamma^\mu\psi]\right\}.}
$$

There is no integration over $B_\mu$. The [gauge covariant derivative](../../../../gauge-covariant-derivative.md) is $\partial_\mu-iB_\mu$, so the simultaneous transformations are

$$
\psi'=e^{i\alpha(x)}\psi,\qquad
\bar\psi'=\bar\psi e^{-i\alpha(x)},\qquad
B'_\mu=B_\mu+\partial_\mu\alpha.
$$

The kinetic term changes by $-j^\mu\partial_\mu\alpha$ and the source term changes by $+j^\mu\partial_\mu\alpha$. The [action](../../../../action.md) is therefore invariant, exactly for finite $\alpha$ as well as infinitesimally. Changing integration variables and using the invariant [functional measure](../../../../functional-measure.md) from part [c](../c.md) proves the [background gauge invariance of a current generating functional](../../../../background-gauge-invariance-of-a-current-generating-functional.md):

$$
\boxed{Z[B+\partial\alpha]=Z[B].}
$$

The allowed transformations preserve the vacuum [boundary conditions](../../../../boundary-condition.md). Its infinitesimal version is $\partial_\mu\delta Z/\delta B_\mu=0$. Because $B_\mu$ is only a source, this statement needs no [gauge fixing](../../../../gauge-fixing.md) or photon kinetic term. The absence of a vector [gauge anomaly](../../../../gauge-anomaly.md) is essential to the change-of-variables argument.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

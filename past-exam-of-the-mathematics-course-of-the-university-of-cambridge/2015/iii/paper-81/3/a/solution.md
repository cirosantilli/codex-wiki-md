<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Hamiltonian](../../../../../../hamiltonian.md) $p^2/(2m)+V(q)$, the real-time [configuration-space path integral](../../../../../../configuration-space-path-integral.md) is

$$
\langle q_f|e^{-iHt/\hbar}|q_i\rangle=\int_{q(0)=q_i}^{q(t)=q_f}\mathcal Dq\,\exp\left[\frac i\hbar\int_0^t\left(\frac m2\dot q^2-V(q)\right)dt'\right],
$$

with its measure defined by time slicing. [Wick rotation](../../../../../../wick-rotation.md) gives the [Euclidean path integral](../../../../../../euclidean-path-integral.md) and the thermal trace.

For the [infinite square well](../../../../../../infinite-square-well.md) on $(0,L)$, the [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) select the normalized [energy eigenstates](../../../../../../energy-eigenstate.md)

$$
\psi_n(q)=\sqrt{\frac2L}\sin\frac{n\pi q}{L},\qquad E_n=\frac{\hbar^2\pi^2n^2}{2mL^2},\qquad n=1,2,\ldots.
$$

There is no $n=0$ state: the corresponding sine is identically zero. Taking the [trace](../../../../../../matrix-trace.md) in this [orthonormal basis](../../../../../../orthonormal-basis.md) gives the [canonical partition function](../../../../../../canonical-partition-function.md)

$$
\boxed{Z(\beta)=\sum_{n=1}^\infty\exp\left(-\frac{\beta\hbar^2\pi^2n^2}{2mL^2}\right)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

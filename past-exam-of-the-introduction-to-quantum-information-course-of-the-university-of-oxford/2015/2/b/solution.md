<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the given [pure state](../../../../pure-state.md) in the ordered [computational basis](../../../../computational-basis.md) $00,01,10,11$:

$$
|\psi\rangle=\frac1{\sqrt3}|00\rangle-\frac1{\sqrt6}|01\rangle
+\frac1{\sqrt3}|10\rangle+\frac1{\sqrt6}|11\rangle,
\qquad
v=\frac1{\sqrt6}\begin{pmatrix}\sqrt2\\-1\\\sqrt2\\1\end{pmatrix}.
$$

The coefficients have squared magnitudes $1/3,1/6,1/3,1/6$, summing to one. The [density matrix](../../../../density-matrix-split.md) is the [outer product](../../../../outer-product.md) $vv^\dagger$, not the diagonal matrix of these four [probabilities](../../../../probability.md): its off-diagonal entries retain [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md). Therefore

$$
\boxed{\rho=|\psi\rangle\langle\psi|
=\frac16\begin{pmatrix}
2&-\sqrt2&2&\sqrt2\\
-\sqrt2&1&-\sqrt2&-1\\
2&-\sqrt2&2&\sqrt2\\
\sqrt2&-1&\sqrt2&1
\end{pmatrix}.}
$$

The [outer product](../../../../outer-product.md) is a [Hermitian matrix](../../../../hermitian-operator.md) and is [positive semidefinite](../../../../positive-semidefinite-matrix.md): $u^\dagger\rho u=|v^\dagger u|^2\geq0$. Its [trace](../../../../matrix-trace.md) is one, and $\rho^2=\rho$, as required for a [pure state](../../../../pure-state.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

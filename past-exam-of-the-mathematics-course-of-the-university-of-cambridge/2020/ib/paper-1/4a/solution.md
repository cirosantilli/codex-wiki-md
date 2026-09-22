<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

An operator $Q$ is Hermitian when

$$
\langle\phi,Q\psi\rangle=\langle Q\phi,\psi\rangle
$$

on its domain. Hermitian operators represent quantum observables because their expectation values and eigenvalues are real. In a normalized state,

$$
(\Delta Q)_\psi
=\left\langle\bigl(Q-\langle Q\rangle_\psi\bigr)^2
\right\rangle_\psi^{1/2}.
$$

Positivity of the norm of $(Q+i\lambda P)\psi$ for every real $\lambda$ gives

$$
0\leq
\langle Q^2\rangle_\psi
+\lambda\langle i[Q,P]\rangle_\psi
+\lambda^2\langle P^2\rangle_\psi.
$$

The middle expectation is real because $i[Q,P]$ is Hermitian. The discriminant of this quadratic is nonpositive, so

$$
\langle Q^2\rangle_\psi\langle P^2\rangle_\psi
\geq\frac14|\langle i[Q,P]\rangle_\psi|^2.
$$

Apply this to the centered operators $Q-\langle Q\rangle_\psi$ and $P-\langle P\rangle_\psi$, whose [commutator](../../../../../commutator.md) is still $[Q,P]$. This yields the [Robertson uncertainty principle](../../../../../robertson-uncertainty-principle.md)

$$
\boxed{(\Delta Q)_\psi(\Delta P)_\psi
\geq\frac12|\langle i[Q,P]\rangle_\psi|}.
$$

Noncommuting observables therefore cannot both have arbitrarily sharply concentrated measurement distributions in the same state.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

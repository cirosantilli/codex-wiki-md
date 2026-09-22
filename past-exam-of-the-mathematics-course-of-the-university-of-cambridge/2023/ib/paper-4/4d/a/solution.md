<h1 id="4d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [expectation value](../../../../../../expectation-value.md) as

$$
\langle O\rangle_\psi=\langle\psi|O|\psi\rangle.
$$

Differentiating and retaining the possible explicit time dependence of the [observable](../../../../../../observable.md) gives

$$
\frac d{dt}\langle O\rangle_\psi
=\langle\dot\psi|O|\psi\rangle
+\left\langle\psi\middle|\frac{\partial O}{\partial t}\middle|\psi\right\rangle
+\langle\psi|O|\dot\psi\rangle.
$$

The [Schrödinger equation](../../../../../../schrodinger-equation.md) and its adjoint are

$$
i\hbar|\dot\psi\rangle=H|\psi\rangle,
\qquad
-i\hbar\langle\dot\psi|=\langle\psi|H,
$$

where the [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) is Hermitian. Substitution yields

$$
\begin{aligned}
\frac d{dt}\langle O\rangle_\psi
&=\frac i\hbar\langle\psi|HO|\psi\rangle
-\frac i\hbar\langle\psi|OH|\psi\rangle
+\left\langle\frac{\partial O}{\partial t}\right\rangle_\psi\\
&=\boxed{\frac i\hbar\langle[H,O]\rangle_\psi
+\left\langle\frac{\partial O}{\partial t}\right\rangle_\psi}.
\end{aligned}
$$

This is the [proof of Ehrenfest theorem from the Schrodinger equation](../../../../../../proof-of-ehrenfest-theorem-from-the-schrodinger-equation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4D](../../4d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

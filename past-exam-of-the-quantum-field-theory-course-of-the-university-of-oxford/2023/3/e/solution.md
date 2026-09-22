<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First conjugate the [Dirac equation](../../../../dirac-equation.md): $(-i\gamma^{\mu*}\partial_\mu-m)\psi^*=0$. A matrix $\Gamma$ taking $\psi^*$ into another solution of the same [Dirac equation](../../../../dirac-equation.md) must obey

$$
\gamma^\mu\Gamma=-\Gamma\gamma^{\mu*}.
$$

Because $\gamma^1$ anticommutes with the real $\gamma^0,\gamma^2$ and commutes with the purely imaginary $\gamma^1$, a unitary choice is

$$
\boxed{\Gamma=\gamma^1=i\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
\psi_C=\gamma^1\psi^*.}
$$

Any constant overall phase is equally valid. To verify invariance of the [action](../../../../action.md), rather than only of its equation, keep the [fermion](../../../../fermion.md) exchange signs. Define the [charge-conjugation matrix](../../../../charge-conjugation-matrix.md) $C=\Gamma\gamma^0=\sigma_2$. It obeys

$$
C^T=-C,\qquad C^{-1}=C,\qquad
C^{-1}\gamma^\mu C=-(\gamma^\mu)^T,
\qquad
\psi_C=C\bar\psi^T,\quad \bar\psi_C=-\psi^TC^{-1}.
$$

For a classical [Grassmann field](../../../../grassmann-field.md), interchanging two components contributes a minus sign; equivalently use [normal ordering](../../../../normal-ordering.md) for quantum [fermionic operators](../../../../fermionic-operator.md). Thus

$$
\bar\psi_C\psi_C=-\psi^T\bar\psi^T=\bar\psi\psi,
$$

and

$$
\bar\psi_Ci\gamma^\mu\partial_\mu\psi_C
=i\psi^T(\gamma^\mu)^T(\partial_\mu\bar\psi)^T
=-i(\partial_\mu\bar\psi)\gamma^\mu\psi
=\bar\psi i\gamma^\mu\partial_\mu\psi
-i\partial_\mu(\bar\psi\gamma^\mu\psi).
$$

The last term integrates to a boundary term, vanishing with the usual decay or compatible boundary conditions. Both the [kinetic term](../../../../kinetic-term.md) and the [Dirac mass term](../../../../dirac-mass-term.md) therefore leave $S$ invariant under [charge conjugation](../../../../charge-conjugation.md). Treating the components as commuting numbers would give the wrong mass-bilinear sign; the [fermion](../../../../fermion.md) statistics is essential.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

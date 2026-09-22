<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $x_P=(t,-x,y)$ and $U_P=\gamma^1$. Since $U_P^\dagger=-\gamma^1$ and $\gamma^0\gamma^1\gamma^0=-\gamma^1$, the [Dirac adjoint](../../../../dirac-adjoint.md) transforms as

$$
\bar\psi'(x)=\psi^\dagger(x_P)(-\gamma^1)\gamma^0
=\bar\psi(x_P)\gamma^1.
$$

The [chain rule](../../../../chain-rule.md) gives $\partial_\mu\psi(x_P)=r_\mu(\partial_\mu\psi)(x_P)$, with $(r_0,r_1,r_2)=(1,-1,1)$ and no sum in this formula. The [Clifford algebra](../../../../clifford-algebra.md) gives

$$
\gamma^1\gamma^0\gamma^1=\gamma^0,\qquad
\gamma^1\gamma^1\gamma^1=-\gamma^1,\qquad
\gamma^1\gamma^2\gamma^1=\gamma^2.
$$

Multiplication by $r_\mu$ therefore restores each [kinetic term](../../../../kinetic-term.md):

$$
\bar\psi'i\gamma^\mu\partial_\mu\psi'
=\bar\psi(x_P)i\gamma^\mu(\partial_\mu\psi)(x_P).
$$

However, the [Dirac scalar bilinear](../../../../dirac-scalar-bilinear.md) changes sign because $(\gamma^1)^2=-I_2$:

$$
\bar\psi'\psi'=-\bar\psi(x_P)\psi(x_P).
$$

Changing variables in the [action](../../../../action.md) has unit absolute [Jacobian determinant](../../../../jacobian-determinant.md). Hence

$$
\boxed{S_m\xrightarrow{P}S_{-m}:\quad S_{\rm kin}\to S_{\rm kin},\quad
-m\int\bar\psi\psi\to+m\int\bar\psi\psi.}
$$

A nonzero [Dirac mass term](../../../../dirac-mass-term.md) for this single two-component field breaks [parity symmetry in quantum field theory](../../../../parity-symmetry-in-quantum-field-theory.md) with the specified transformation.

## ↑ Ancestors (12)

1. [C](../c.md)
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

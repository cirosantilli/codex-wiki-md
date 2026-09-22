<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The specified [time reversal](../../../../t-symmetry.md) includes complex conjugating $i\gamma^\mu\partial_\mu$; omitting that operation changes the answer. Put $x_T=(-t,x,y)$, $U_T=\gamma^2$, and $(r_0,r_1,r_2)=(-1,1,1)$. As in [c](../c.md), the [Dirac adjoint](../../../../dirac-adjoint.md) in the source's transformed bilinear is $\bar\psi'(x)=\bar\psi(x_T)\gamma^2$. The conjugated [Dirac operator](../../../../dirac-operator.md) has coefficient matrices

$$
(i\gamma^0)^*=-i\gamma^0,\qquad
(i\gamma^1)^*=+i\gamma^1,\qquad
(i\gamma^2)^*=-i\gamma^2.
$$

Combining these coefficients with the [chain rule](../../../../chain-rule.md) signs and the [Clifford algebra](../../../../clifford-algebra.md) gives, without summing over $\mu$,

$$
\gamma^2(i\gamma^\mu)^*\gamma^2r_\mu=i\gamma^\mu
\quad(\mu=0,1,2).
$$

For example the time coefficient is $\gamma^2(-i\gamma^0)\gamma^2(-1)=i\gamma^0$, and the second spatial coefficient is $\gamma^2(-i\gamma^2)\gamma^2=i\gamma^2$. Thus the [kinetic term](../../../../kinetic-term.md) is invariant. The real [Dirac mass term](../../../../dirac-mass-term.md) again reverses sign since $\bar\psi'\psi'=\bar\psi(\gamma^2)^2\psi=-\bar\psi\psi$. The spacetime integration has unit absolute [Jacobian determinant](../../../../jacobian-determinant.md), so

$$
\boxed{T:S_m\mapsto S_{-m},\qquad TP:S_m\mapsto S_m.}
$$

Each operation reverses the sign of the mass, while their composition reverses it twice and preserves the [kinetic term](../../../../kinetic-term.md). In an operator formulation the complex conjugation of coefficients expresses the [antiunitary operator](../../../../antiunitary-operator.md) character of [time reversal](../../../../t-symmetry.md); the transformation must not be treated as an ordinary unitary substitution with all $i$'s held fixed. These statements concern the stated free [action](../../../../action.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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

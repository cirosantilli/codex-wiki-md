<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $u=A\psi$, $v=B\psi$ and $z=\langle u,v\rangle$. The [self-adjointness](../../../../self-adjoint-operator.md) of $A,B$ implies

$$
z=\langle\psi,AB\psi\rangle,\qquad \overline z=\langle\psi,BA\psi\rangle,\qquad \mathbb E_\psi(C)=-i(z-\overline z)=2\operatorname{Im}z.
$$

The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) followed by $|z|^2\geq(\operatorname{Im}z)^2$ gives

$$
\mathbb E_\psi(A^2)\mathbb E_\psi(B^2)=\|u\|^2\|v\|^2\geq|z|^2\geq(\operatorname{Im}z)^2=\boxed{\frac14\bigl(\mathbb E_\psi(C)\bigr)^2}.
$$

Both inequalities must be equalities. The exact conditions are **$A\psi$ and $B\psi$ are linearly dependent, and $\operatorname{Re}\langle A\psi,B\psi\rangle=0$**. Equivalently, equality holds if either vector is zero; when both are nonzero it holds precisely when

$$
\boxed{B\psi=i\lambda A\psi\quad\text{for some real }\lambda\ne0.}
$$

The zero-vector cases matter: they saturate the inequality but cannot all be expressed by solving for $B\psi$ as a multiple of $A\psi$. The real-part condition can also be written $\mathbb E_\psi(AB+BA)=0$, using the [anticommutator](../../../../anticommutator.md). This is the [uncentered second-moment commutator inequality](../../../../uncentered-second-moment-commutator-inequality.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

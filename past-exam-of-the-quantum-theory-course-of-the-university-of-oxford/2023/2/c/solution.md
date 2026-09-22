<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [canonical commutation relations](../../../../canonical-commutation-relation.md)

$$
[X_j,P_k]=i\hbar\delta_{jk}I,\qquad [X_j,X_k]=[P_j,P_k]=0.
$$

Writing $c_j=\sqrt{m\omega_j/(2\hbar)}$, $d_j=1/\sqrt{2m\hbar\omega_j}$, direct expansion of the [commutator](../../../../commutator.md) gives

$$
[a_{j,-},a_{k,+}]=\hbar(c_jd_k+d_jc_k)\delta_{jk}I
=\boxed{\delta_{jk}I}.
$$

The [Fock vacuum](../../../../fock-vacuum.md) $\psi_{0,0}$ is annihilated by both $a_{j,-}$. Successive [creation operators](../../../../creation-operator.md) generate

$$
\psi_{n_1,n_2}\propto(a_{1,+})^{n_1}(a_{2,+})^{n_2}\psi_{0,0}.
$$

Hence, in the order of part (a), the six [energy eigenstates](../../../../energy-eigenstate.md) are proportional to

$$
\boxed{\psi_{0,0},\quad a_{1,+}\psi_{0,0},\quad a_{2,+}\psi_{0,0},\quad
(a_{1,+})^2\psi_{0,0},\quad a_{1,+}a_{2,+}\psi_{0,0},\quad(a_{2,+})^2\psi_{0,0}.}
$$

If the [Fock vacuum](../../../../fock-vacuum.md) has unit [norm](../../../../norm.md), dividing the general expression by $\sqrt{n_1!n_2!}$ gives normalized [number states](../../../../number-state.md). Normalization is not required here, but using this convention makes the later change of basis unambiguous.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

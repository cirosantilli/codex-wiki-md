<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each complex fermion define two [Majorana fermion operators](../../../../../../majorana-fermion-operator.md)

$$
c_{2j-1}=a_j+a_j^\dagger,
\qquad
c_{2j}=-i(a_j-a_j^\dagger).
$$

They obey $c_r^\dagger=c_r$, $\{c_r,c_s\}=2\delta_{rs}$, and $a_j=(c_{2j-1}+ic_{2j})/2$. Substituting these inverse relations expands every hopping and pairing monomial as a bilinear in the $c_r$. Diagonal terms $c_r^2=1$ contribute only a constant.

For $r\ne s$, $c_rc_s$ is anti-Hermitian. Hermiticity of the original [quadratic fermion Hamiltonian](../../../../../../quadratic-fermion-hamiltonian.md) therefore makes its coefficient purely imaginary, so it can be written $iA_{rs}$ with $A_{rs}$ real. Since

$$
\sum_{rs}A_{rs}c_rc_s
=\frac12\sum_{rs}(A_{rs}-A_{sr})c_rc_s
+\frac12\operatorname{tr}A,
$$

the symmetric part again changes only the constant. Absorbing conventional factors into $A$ gives

$$
\boxed{H=i\sum_{rs}A_{rs}c_rc_s+\text{constant},
\qquad A^T=-A,
\qquad A\in M_{2n}(\mathbb R).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

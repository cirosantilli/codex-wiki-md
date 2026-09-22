<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**The fundamental case.** Set $\langle\phi\rangle=v e_4$, where $v\ne0$. Fixing this [vector](../../../../vector.md) forces the fourth column of a [unitary matrix](../../../../unitary-matrix.md) to be $e_4$, and hence also fixes its fourth row. The remaining three-by-three block has [determinant](../../../../determinant.md) one. Therefore

$$
\boxed{\operatorname{Stab}(ve_4)=\{\operatorname{diag}(W,1):W\in SU(3)\}=H_3.}
$$

Every nonzero complex [vector](../../../../vector.md) can be brought to this form by an [SU(4)](../../../../su-4-group.md) transformation: complete its normalized direction to a unitary [basis](../../../../basis.md) and adjust the phase of a complementary [basis vector](../../../../basis-vector.md) to obtain [determinant](../../../../determinant.md) one. Thus a generic nonzero fundamental [vacuum expectation value](../../../../vacuum-expectation-value.md) has a conjugate of $H_3$ as its exact unbroken [subgroup](../../../../subgroup.md). The particular embedded $H_3$ of the question is fixed only when the [vacuum expectation value](../../../../vacuum-expectation-value.md) lies along $e_4$.

**The antisymmetric case.** With $\epsilon=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$, take

$$
\langle A\rangle=\begin{pmatrix}a\epsilon&0\\0&b\epsilon\end{pmatrix}.
$$

Since $V\epsilon V^T=\epsilon$ for $V\in SU(2)$, this [antisymmetric tensor](../../../../antisymmetric-tensor.md) is fixed by $H_2$ for every $a,b$. Its transformation is $A\mapsto UAU^T$, so any stabilizing $U$ also preserves

$$
AA^\dagger=\operatorname{diag}(|a|^2I_2,|b|^2I_2).
$$

If $|a|\ne|b|$, its two [eigenspaces](../../../../eigenspace.md) force $U=\operatorname{diag}(V,\widetilde V)$ with unitary two-by-two blocks. For each nonzero block, $V\epsilon V^T=(\det V)\epsilon$ forces the block [determinant](../../../../determinant.md) to be one. If one block is zero, the [SU(4)](../../../../su-4-group.md) [determinant](../../../../determinant.md) condition forces the other block [determinant](../../../../determinant.md) to be one as well. Hence

$$
\boxed{|a|\ne|b|\quad\Longrightarrow\quad\operatorname{Stab}(\langle A\rangle)=H_2.}
$$

The [unitary skew-diagonalization of an antisymmetric matrix](../../../../unitary-skew-diagonalization-of-an-antisymmetric-matrix.md) shows that a generic complex $\mathbf6$ has two distinct paired [singular values](../../../../singular-value.md); choosing an [SU(4)](../../../../su-4-group.md) rather than a $U(4)$ [basis](../../../../basis.md) merely leaves an allowed overall phase in $a,b$. Thus its generic [stabilizer](../../../../stabilizer-subgroup.md) is conjugate to $H_2$.

If instead $|a|=|b|\ne0$, the form is proportional, up to unitary coordinates and phases, to a nondegenerate standard symplectic form. Its [stabilizer](../../../../stabilizer-subgroup.md) is the [compact symplectic group](../../../../compact-symplectic-group.md) $USp(4)$, of [dimension](../../../../dimension-vector-space.md) ten, containing $H_2$ properly. The explicit choice $a=b=1$ is a concrete counterexample to inferring an exact $H_2$ [stabilizer](../../../../stabilizer-subgroup.md) from the existence of two singlets alone. For a real $\mathbf6$, the [real structure of the SU4 exterior square](../../../../real-structure-of-the-su4-exterior-square.md) imposes $b=\bar a$ in this form, so these equal magnitudes are compulsory. Every nonzero real $\mathbf6$ therefore has the larger [compact symplectic group](../../../../compact-symplectic-group.md) [stabilizer](../../../../stabilizer-subgroup.md). The zero [vacuum expectation value](../../../../vacuum-expectation-value.md) preserves all of $SU(4)$.

**The adjoint cases.** The $H_2$-fixed and $H_3$-fixed traceless [matrices](../../../../matrix.md) have respectively the forms

$$
X_2=a\operatorname{diag}(1,1,-1,-1),\qquad
X_3=a\operatorname{diag}(1,1,1,-3),\qquad a\ne0.
$$

For a Hermitian adjoint [scalar field](../../../../scalar-field.md), choose $a$ real. More generally a complex $a$ gives the same [stabilizers](../../../../stabilizer-subgroup.md). The repeated [eigenvalues](../../../../eigenvalue.md) imply

$$
\boxed{\operatorname{Stab}(X_2)=S(U(2)\times U(2)),\qquad
\operatorname{Stab}(X_3)=S(U(3)\times U(1)).}
$$

Here $S$ means that the product of the block [determinants](../../../../determinant.md) is one. These [groups](../../../../group-split.md) contain respectively $H_2$ and $H_3$, together with an additional continuous $U(1)$. Explicit extra transformations are $\operatorname{diag}(e^{it}I_2,e^{-it}I_2)$ and $\operatorname{diag}(e^{it}I_3,e^{-3it})$. They commute with $X_2$ and $X_3$ for every $t$, proving that neither exact endpoint $H_2$ or $H_3$ occurs for a single adjoint [vacuum expectation value](../../../../vacuum-expectation-value.md).

Nor do these larger [subgroups](../../../../subgroup.md) survive for a generic Hermitian traceless [matrix](../../../../matrix.md): four distinct [eigenvalues](../../../../eigenvalue.md) leave only the [maximal torus](../../../../maximal-torus.md) $U(1)^3$. For a generic complex adjoint [matrix](../../../../matrix.md), there need not even be a continuous [stabilizer](../../../../stabilizer-subgroup.md); generically its unitary [centralizer](../../../../centralizer.md) is just the [centre of a group](../../../../center-of-a-group.md) $\mathbb Z_4$. Thus the displayed degenerate adjoint directions are special. All these statements concern the [stabilizer](../../../../stabilizer-subgroup.md) of a possible [vacuum expectation value](../../../../vacuum-expectation-value.md); no unspecified [scalar potential](../../../../scalar-potential.md) can be assumed to select a particular direction or a particular reality condition.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)

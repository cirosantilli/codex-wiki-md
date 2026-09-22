<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the unnormalized [Choi matrix](../../../../../../choi-matrix.md)

$$
J_\Phi=(\Phi_A\otimes\mathrm{id}_B)(|\widetilde\Psi_{AB}\rangle\langle\widetilde\Psi_{AB}|).
$$

It is positive because $\Phi_A$ is a [completely positive map](../../../../../../completely-positive-map.md). Take its spectral decomposition, absorbing square roots of nonzero eigenvalues into the vectors:

$$
J_\Phi=\sum_{k=1}^r|v_k\rangle\langle v_k|,\qquad r=\operatorname{rank}J_\Phi\leq d^2.
$$

Expand $|v_k\rangle=\sum_{i,j}v_{k,ij}|i\rangle_A|j\rangle_B$ and define the [Kraus operator](../../../../../../kraus-operator.md) $A_k$ by $(A_k)_{ij}=v_{k,ij}$. Equivalently,

$$
|v_k\rangle=(A_k\otimes I_B)|\widetilde\Psi_{AB}\rangle.
$$

The preceding [relative state](../../../../../../relative-state-of-a-bipartite-vector.md) identity then gives $(I\otimes\langle\phi_B^*|)v_k=A_k\phi_A$. Inserting the spectral decomposition into the stated reconstruction identity yields

$$
\Phi_A(|\phi\rangle\langle\phi|)=\sum_kA_k|\phi\rangle\langle\phi|A_k^\dagger.
$$

The conjugated index vector is required here; it is present in the PDF but missing in the converted TeX version of this identity.

Rank-one projectors span all operators by polarization. Explicitly, putting $P(w)=|w\rangle\langle w|$ gives

$$
4|u\rangle\langle v|=P(u+v)-P(u-v)+iP(u+iv)-iP(u-iv).
$$

Thus linearity extends the equality to every $X\in\mathcal B(\mathcal H_A)$:

$$
\boxed{\Phi_A(X)=\sum_kA_kXA_k^\dagger.}
$$

Finally trace preservation and cyclicity of the trace give

$$
\operatorname{Tr}X=\operatorname{Tr}\Phi_A(X)=\operatorname{Tr}\left[X\sum_kA_k^\dagger A_k\right].
$$

For pure-projector inputs this says the Hermitian operator $\sum_kA_k^\dagger A_k-I$ has zero expectation on every vector, so it vanishes. Therefore

$$
\boxed{\sum_kA_k^\dagger A_k=I_A.}
$$

This is the [spectral Kraus decomposition](../../../../../../spectral-kraus-decomposition.md). Using a normalized [Choi state](../../../../../../choi-state.md) $J_\Phi/d$ instead would require the extra factor $\sqrt d$ when reshaping its eigenvectors into Kraus operators.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

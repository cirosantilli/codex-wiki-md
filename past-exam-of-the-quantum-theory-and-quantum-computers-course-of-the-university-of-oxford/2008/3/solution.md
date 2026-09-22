<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [density operator](../../../density-matrix-split.md) is a positive self-adjoint [trace-class operator](../../../trace-class-operator.md) with $\boxed{\operatorname{Tr}\rho=1}$. A finite [expectation](../../../expected-value-split.md) is $\boxed{\langle A\rangle_\rho=\operatorname{Tr}(\rho A)}$. It represents a [pure state](../../../pure-state.md) exactly when $\rho=|v\rangle\langle v|$ for a unit vector, equivalently $\rho^2=\rho$ or $\operatorname{Tr}\rho^2=1$.

For a [finite-dimensional](../../../finite-dimensional-vector-space.md) [spectral decomposition](../../../spectral-decomposition.md) $\rho=\sum_jp_j|v_j\rangle\langle v_j|$, introduce an auxiliary space with [orthonormal](../../../orthonormal-set.md) vectors $f_j$ and use the enlarged space $\mathcal K=\mathcal H\otimes\mathcal E$. Define

$$
\Omega_\rho=\sum_j\sqrt{p_j}\,v_j\otimes f_j,\qquad\widetilde A=A\otimes I.
$$

Then $\|\Omega_\rho\|^2=\sum p_j=1$ and $\langle\Omega_\rho,\widetilde A\Omega_\rho\rangle=\sum p_j\langle v_j,Av_j\rangle=\operatorname{Tr}(\rho A)$. This [purification](../../../purification-of-a-density-operator.md) shows that subsystem mixedness can arise from [entanglement](../../../entangled-state.md) with an unobserved environment [even](../../../even-function.md) when the total state is pure. Subsystem measurements alone cannot distinguish these two descriptions.

A nonzero pure bipartite vector is entangled when it cannot be written as a [tensor product](../../../tensor-product.md) of two vectors; equivalently its [Schmidt rank](../../../schmidt-rank.md) exceeds one. For mixed bipartite states, [entanglement](../../../entangled-state.md) means absence of a convex decomposition into product [density operators](../../../density-matrix-split.md).

For the nonorthogonal expansion in the question, the unnormalized reduced operator is

$$
\boxed{S_1=\sum_{j,k}\langle\eta_k,\eta_j\rangle\,|\xi_j\rangle\langle\xi_k|.}
$$

Indeed $\langle\Psi,(A\otimes I)\Psi\rangle=\sum_{j,k}\langle\xi_k,A\xi_j\rangle\langle\eta_k,\eta_j\rangle=\operatorname{Tr}(AS_1)$. Positivity follows because $\langle v,S_1v\rangle=\|\sum_j\langle v,\xi_j\rangle\eta_j\|^2\geq0$, and $\operatorname{Tr}S_1=\|\Psi\|^2=:Z$. Thus $\boxed{\rho_1=S_1/Z}$ is a [density operator](../../../density-matrix-split.md); if $\Psi$ is already [normalized](../../../normalization.md), $Z=1$. The Gram factors cannot be dropped merely because the vectors are called bases. For unnormalized $\Psi$, physical [expectations](../../../expected-value-split.md) likewise divide its raw quadratic form by $Z$.

For the [Schmidt decomposition](../../../schmidt-decomposition.md) diagonalize $S_1$ in an [orthonormal](../../../orthonormal-set.md) [basis](../../../basis.md) $\xi_j$ with its positive [eigenvalues](../../../eigenvalue.md) $c_j^2$. Expand $\Psi=\sum_j\xi_j\otimes w_j$ with $w_j=(\langle\xi_j|\otimes I)\Psi$. The reduced [matrix](../../../matrix.md) gives $\langle w_k,w_j\rangle=c_j^2\delta_{jk}$. Therefore $\eta_j=w_j/c_j$ are [orthonormal](../../../orthonormal-set.md) and

$$
\boxed{\Psi=\sum_{j:c_j>0}c_j\xi_j\otimes\eta_j.}
$$

Zero-[eigenvalue](../../../eigenvalue.md) components vanish because their squared [norms](../../../norm.md) are zero. This proves the decomposition for an arbitrary nonzero vector; the zero vector uses the empty sum. For a unit vector $\sum c_j^2=1$.

In the numerical example the coefficient [matrix](../../../matrix.md) in the two product bases is $C=\begin{pmatrix}1&2&3\\0&1&2\end{pmatrix}$. Taking the first-subsystem [trace](../../../matrix-trace.md) yields

$$
\boxed{S_2=C^{\mathsf T}C=\begin{pmatrix}1&2&3\\2&5&8\\3&8&13\end{pmatrix}.}
$$

The vector $(1,-2,1)^{\mathsf T}$ is in its [nullspace](../../../kernel-of-a-linear-map-split.md), so [rank](../../../rank-one-quadratic-form.md) is at most two; its leading $2\times2$ minor has [determinant](../../../determinant.md) one, so $\boxed{\operatorname{rank}S_2=2}$. This is the [rank](../../../rank-one-quadratic-form.md) of $C$ and the [Schmidt rank](../../../schmidt-rank.md), proving [entanglement](../../../entangled-state.md). **The displayed source ket has [norm](../../../norm.md) squared $19$**, and the displayed reduced [matrix](../../../matrix.md) has [trace](../../../matrix-trace.md) $19$. The physical [density operator](../../../density-matrix-split.md) is $\boxed{\rho_2=S_2/19}$; its nonzero [eigenvalues](../../../eigenvalue.md) are $(19\pm\sqrt{337})/38$, since $CC^{\mathsf T}=\begin{pmatrix}14&8\\8&5\end{pmatrix}$. The raw [matrix](../../../matrix.md) is correct for the unnormalized quadratic form actually printed.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2008](../../2008-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

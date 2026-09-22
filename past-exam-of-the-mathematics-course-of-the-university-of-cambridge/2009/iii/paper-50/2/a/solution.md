<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D=\dim\mathcal H_A$ and introduce an isomorphic reference system $R$. Choose a basis $\{|j\rangle\}_{j=1}^D$ and the [maximally entangled state](../../../../../../maximally-entangled-state.md)

$$
|\Omega\rangle_{RA}=\frac1{\sqrt D}\sum_{j=1}^D|j\rangle_R|j\rangle_A.
$$

Complete positivity makes

$$
\omega_{RA}=(\operatorname{id}_R\otimes\Phi)(|\Omega\rangle\langle\Omega|)
$$

a positive [density operator](../../../../../../density-matrix.md). This is the normalized [Choi matrix](../../../../../../choi-matrix.md), with the reference placed first. Its [spectral decomposition](../../../../../../spectral-decomposition.md) can be written

$$
\omega_{RA}=\sum_{\ell=1}^{r}\lambda_\ell|v_\ell\rangle\langle v_\ell|,
\qquad \lambda_\ell>0.
$$

The number $r$ is at most $D^2$.

Here an [index state](../../../../../../index-state.md) is a chosen basis vector $|j\rangle_R$ in the reference. The corresponding [relative state](../../../../../../relative-state-of-a-bipartite-vector.md) of $|v_\ell\rangle$ is the generally unnormalized vector

$$
|\eta_{\ell j}\rangle_A=(\langle j|_R\otimes I_A)|v_\ell\rangle_{RA}.
$$

Thus $|v_\ell\rangle=\sum_j|j\rangle_R|\eta_{\ell j}\rangle_A$. Define a [linear map](../../../../../../linear-map.md) $A_\ell$ by its columns:

$$
A_\ell|j\rangle=\sqrt{D\lambda_\ell}\,|\eta_{\ell j}\rangle.
$$

Then $(I_R\otimes A_\ell)|\Omega\rangle=\sqrt{\lambda_\ell}|v_\ell\rangle$, so

$$
\omega_{RA}=\sum_\ell(I_R\otimes A_\ell)|\Omega\rangle\langle\Omega|(I_R\otimes A_\ell^\dagger).
$$

Expand both sides in reference [matrix units](../../../../../../matrix-unit.md). The block with reference indices $i,j$ on the left is $D^{-1}\Phi(|i\rangle\langle j|)$; on the right it is $D^{-1}\sum_\ell A_\ell|i\rangle\langle j|A_\ell^\dagger$. Since [matrix units](../../../../../../matrix-unit.md) span all operators and $\Phi$ is linear,

$$
\boxed{\Phi(\rho)=\sum_\ell A_\ell\rho A_\ell^\dagger.}
$$

This constructs the [Kraus representation](../../../../../../kraus-representation.md) explicitly from the relative states, rather than assuming it.

Finally, [trace](../../../../../../matrix-trace.md) preservation implies for every [density operator](../../../../../../density-matrix.md) $\rho$ that

$$
\operatorname{Tr}\rho=\operatorname{Tr}\Phi(\rho)
=\operatorname{Tr}\left[\rho\sum_\ell A_\ell^\dagger A_\ell\right].
$$

Taking every rank-one [orthogonal projection](../../../../../../orthogonal-projection.md) as $\rho$ forces the [Hermitian operator](../../../../../../hermitian-operator.md) in brackets to have the same quadratic form as the identity. Therefore

$$
\boxed{\sum_\ell A_\ell^\dagger A_\ell=I.}
$$

The argument is finite-dimensional, as appropriate to the quantum-information setting; a channel with a different output dimension has the same construction with rectangular [Kraus operators](../../../../../../kraus-operator.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

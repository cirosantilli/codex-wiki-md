<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Quantize the real massless [scalar field](../../../../../../scalar-field.md) using the normalized in-modes:

$$
\widehat\phi=\sum_j\left(a_jf_j+a_j^\dagger\bar f_j\right),\qquad[a_j,a_k^\dagger]=\delta_{jk},\qquad a_j|0_{\rm in}\rangle=0.
$$

Use the [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md) convention that is antilinear in its first argument. Mode normalization gives

$$
(f_j,f_k)=\delta_{jk},\qquad(\bar f_j,\bar f_k)=-\delta_{jk},\qquad(f_j,\bar f_k)=0.
$$

The out annihilation operator is $b_i=(p_i,\widehat\phi)$. Applying the [Bogoliubov transformation](../../../../../../bogoliubov-transformation.md) and the negative norm of conjugate modes gives

$$
\boxed{b_i=\sum_j\left(\bar A_{ij}a_j-\bar B_{ij}a_j^\dagger\right).}
$$

Both the complex conjugation and the minus sign follow from the inner-product convention. These operators annihilate the [out-vacuum](../../../../../../out-vacuum.md), but need not annihilate the [in-vacuum](../../../../../../in-vacuum.md). The [particle number operator](../../../../../../number-operator.md) in out-mode $i$ is $N_i^{\rm out}=b_i^\dagger b_i$. In the [in-vacuum](../../../../../../in-vacuum.md), the only nonzero contraction is $\langle0_{\rm in}|a_ja_k^\dagger|0_{\rm in}\rangle=\delta_{jk}$, obtained from the [canonical commutation relation](../../../../../../canonical-commutation-relation.md). Thus

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle=\sum_{j,k}B_{ij}\bar B_{ik}\delta_{jk}=\sum_j|B_{ij}|^2=(BB^\dagger)_{ii}.}
$$

This is [particle number from Bogoliubov coefficients](../../../../../../particle-number-from-bogoliubov-coefficients.md): mixing with negative-frequency in-modes produces out-particles even though no in-particles were present. For continuous mode labels the sum becomes an integral; normalized wave packets make an individual occupation number well-defined. No explicit collapse geometry or thermal spectrum is needed for this conclusion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

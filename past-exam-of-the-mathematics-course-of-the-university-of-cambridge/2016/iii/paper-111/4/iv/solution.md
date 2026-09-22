<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Within each fixed [unitary irreducible representation](../../../../../../unitary-irreducible-representation.md), choose the selected [right singular vectors](../../../../../../right-singular-vector.md) to be [orthonormal](../../../../../../orthonormal-set.md). Their corresponding [left singular vectors](../../../../../../left-singular-vector.md) are also [orthonormal](../../../../../../orthonormal-set.md), even when a [singular value](../../../../../../singular-value.md) is repeated: choose an [orthonormal basis](../../../../../../orthonormal-basis.md) in each eigenspace of $T_\rho^*T_\rho$ and put $B_p=T_\rho A_p/\lambda_p$. Therefore, when $\rho_p=\rho_q$,

$$
\boxed{\operatorname{tr}(U(p)^*U(q))
=\operatorname{tr}(V(p)^*V(q))
=n_p\delta_{pq}}.
$$

This is (iv), with the unnormalized [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) and the [Kronecker delta](../../../../../../kronecker-delta.md). No orthogonality of differently shaped matrices is being asserted.

For the unheaded continuation, partition $b\in\mathbb C^m$ into blocks $b_p\in\mathbb C^{n_p}$. Then

$$
UP(x)^*b=\sum_pU(p)\rho_p(x)^*b_p.
$$

The [Schur averaging of rectangular matrices](../../../../../../schur-averaging-of-rectangular-matrices.md) formula is

$$
\mathbb E_x\rho_p(x)M\rho_q(x)^*
=\begin{cases}(\operatorname{tr}M/n_p)I_{n_p},&\rho_p=\rho_q,\\0,&\rho_p\ne\rho_q,\end{cases}
$$

for any $n_p\times n_q$ matrix $M$. The average is an [intertwiner](../../../../../../intertwiner.md); the [Schur lemma](../../../../../../schur-s-lemma.md) makes it zero for inequivalent [irreducible representations](../../../../../../irreducible-representation.md), and a scalar multiple of the identity for the same representative. The [trace](../../../../../../matrix-trace.md) determines that scalar in the latter case.

Apply this with $M=U(p)^*U(q)$. The [Hilbert-Schmidt inner product](../../../../../../hilbert-schmidt-inner-product.md) normalization just proved gives

$$
\mathbb E_x\rho_p(x)U(p)^*U(q)\rho_q(x)^*
=\begin{cases}I_{n_p},&p=q,\\0,&p\ne q.\end{cases}
$$

Expanding the squared [Euclidean norm](../../../../../../euclidean-norm.md) now yields

$$
\begin{aligned}
\mathbb E_x\|UP(x)^*b\|_2^2
&=\sum_{p,q}b_p^*\mathbb E_x\bigl[\rho_p(x)U(p)^*U(q)\rho_q(x)^*\bigr]b_q\\
&=\sum_p\|b_p\|_2^2
=\boxed{\|b\|_2^2}.
\end{aligned}
$$

Thus the final identity follows from averaging, although $U^*U$ itself need not be the identity. The whole construction is the [spectral inverse theorem for the matrix-valued U2 quantity](../../../../../../spectral-inverse-theorem-for-the-matrix-valued-u2-quantity.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

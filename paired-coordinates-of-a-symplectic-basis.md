# Paired coordinates of a symplectic basis

↑ **Parent:** [Symplectic basis](symplectic-basis.md)

Write [vectors](vector.md) in a [symplectic basis](symplectic-basis.md) as $v=\sum_i(q_i e_i+p_i f_i)$ and $w=\sum_i(Q_i e_i+P_i f_i)$. Their [coordinate vectors](coordinate-vector.md) and the [matrix of a bilinear form](matrix-of-a-bilinear-form.md) are

$$
[v]_{\mathcal B}=\begin{pmatrix}q\\p\end{pmatrix},\qquad
J=\begin{pmatrix}0&I_n\\-I_n&0\end{pmatrix},\qquad
\omega(v,w)=[v]_{\mathcal B}^{T}J[w]_{\mathcal B}
=\sum_{i=1}^n(q_iP_i-p_iQ_i).
$$

Here $I_n$ is the [identity matrix](identity-matrix.md), and $T$ denotes [transpose](transpose.md). The ordering matters: interleaving the [basis](basis.md) as $(e_1,f_1,\ldots,e_n,f_n)$ instead gives a [block diagonal matrix](block-diagonal-matrix.md) with $2\times2$ blocks $\begin{pmatrix}0&1\\-1&0\end{pmatrix}$. Some conventions reverse every $f_i$, giving $-J$ instead. Always check the displayed pairing convention.[§1.1, p. 83: e-then-f basis and its block matrix; the coordinate formula follows by bilinearity](handbook-of-differential-geometry-volume-ii/symplectic-geometry.md)

Over the [real numbers](real-number.md), each summand is the signed [area](surface-area.md) of a [parallelogram](parallelogram.md) in the $(q_i,p_i)$ coordinate plane. For $a=(2,1,1,1)^T$ and $b=(1,1,0,2)^T$, the two signed [areas](surface-area.md) are $-1$ and $1$, so $\omega(a,b)=0$ although the [vectors](vector.md) are [linearly independent](linear-independence.md). The cancellation concerns the [symplectic form](symplectic-form.md); it does not assert that their [dot product](dot-product.md) vanishes. Over a general [field](field.md), the same [determinant](determinant.md) formula is algebraic, without a signed geometric interpretation.

<a id="image-paired-coordinate-planes-and-the-pairing-matrix-of-a-four-dimensional-symplectic-basis"></a>
![](symplectic-paired-coordinate-areas.png)

**[Figure 7](#image-paired-coordinate-planes-and-the-pairing-matrix-of-a-four-dimensional-symplectic-basis). Paired coordinate planes and the pairing matrix of a four-dimensional symplectic basis**. The two projected parallelograms have signed areas minus one and plus one, which cancel. The matrix uses the e-then-f ordering; all self-pairings are zero.

## ↑ Ancestors (9)

1. [Symplectic basis](symplectic-basis.md)
2. [Symplectic vector space](symplectic-vector-space.md)
3. [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
4. [Bilinear form](bilinear-form-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

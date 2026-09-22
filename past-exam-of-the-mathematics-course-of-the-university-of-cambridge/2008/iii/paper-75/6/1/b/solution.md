<h1 id="6/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The dual vectors are the [Riesz dual basis in an inner product space](../../../../../../../riesz-dual-basis-in-an-inner-product-space.md), and lie in $\mathcal U_n$ itself. Take the convention that the [inner product](../../../../../../../inner-product.md) is conjugate-linear in its first argument; in a real space the conjugations can simply be omitted. Since the $u_j$ form a [basis](../../../../../../../basis.md), their [Gram matrix](../../../../../../../gram-matrix.md) $G$ is positive definite and invertible. Let $B=G^{-1}$ and put

$$
\widehat u_k=\sum_{\ell=1}^n b_{\ell k}u_\ell.
$$

The proposed vectors satisfy

$$
(u_i,\widehat u_k)=\sum_\ell G_{i\ell}b_{\ell k}=(GB)_{ik}=\delta_{ik}.
$$

They therefore give the unique dual family within $\mathcal U_n$. Their own [Gram matrix](../../../../../../../gram-matrix.md) is

$$
\bigl((\widehat u_j,\widehat u_k)\bigr)_{j,k}=B^*GB.
$$

The inverse of a Hermitian positive-definite [matrix](../../../../../../../matrix.md) is Hermitian, so $B^*=B$. Using $GB=I$ gives $B^*GB=B$. Consequently

$$
\boxed{(\widehat u_j,\widehat u_k)=b_{jk}.}
$$

For a real space this is the familiar identity $B^TGB=B$. If the opposite complex inner-product convention is adopted, conjugate the coefficients in the dual-vector formula; the stated identity remains the same. Requiring the dual vectors to lie in $\mathcal U_n$ is essential: arbitrary additions perpendicular to $\mathcal U_n$ preserve the pairings with $u_i$ but alter the Gram [matrix](../../../../../../../matrix.md) of the dual vectors.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [6](../../../6.md)
4. [Paper 75](../../../../paper-75-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="6/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the convention that the [inner product](../../../../../../../inner-product.md) is conjugate-linear in its first argument; the real case is the same without conjugates. [Linear independence](../../../../../../../linear-independence.md) makes the [Gram matrix](../../../../../../../gram-matrix.md) $G$ positive definite, so $B=G^{-1}$ exists and is Hermitian. Define the [Riesz dual basis in an inner product space](../../../../../../../riesz-dual-basis-in-an-inner-product-space.md) within $\mathcal U_n$ by

$$
\widehat u_k=\sum_{l=1}^n b_{lk}u_l.
$$

Then $(u_i,\widehat u_k)=\sum_lG_{il}b_{lk}=\delta_{ik}$. Its own Gram entries are

$$
(\widehat u_j,\widehat u_k)=\sum_{l,m}\overline{b_{lj}}G_{lm}b_{mk}
=(B^*GB)_{jk}=B_{jk}.
$$

Hence **the inverse [Gram matrix](../../../../../../../gram-matrix.md) is the [Gram matrix](../../../../../../../gram-matrix.md) of the dual vectors**:

$$
\boxed{b_{jk}=(\widehat u_j,\widehat u_k).}
$$

The dual vectors are required to lie in $\mathcal U_n$; adding arbitrary vectors orthogonal to that subspace would preserve the displayed biorthogonality but would destroy this conclusion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [6](../../../6.md)
4. [Paper 69](../../../../paper-69-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

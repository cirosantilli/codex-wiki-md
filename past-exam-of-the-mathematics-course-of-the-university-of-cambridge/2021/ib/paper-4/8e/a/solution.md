<h1 id="8e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Hermitian form](../../../../../../hermitian-form.md) is a [sesquilinear form](../../../../../../sesquilinear-form.md) $H:V\times V\to\mathbb C$ such that

$$
H(v,w)=\overline{H(w,v)}.
$$

Use the convention that $H$ is linear in its first argument and conjugate-linear in its second. Its [matrix](../../../../../../matrix-of-a-hermitian-form.md) in the basis $(v_1,\ldots,v_n)$ is

$$
A_{ij}=H(v_i,v_j).
$$

If $v=\sum_i x_iv_i$ and $w=\sum_jy_jv_j$, then

$$
H(v,w)=x^TA\overline y.
$$

Since $w_i=\sum_jp_{ij}v_j$, the coordinate row of each new basis vector is a row of $P$. Direct substitution gives

$$
H(w_i,w_k)=\sum_{j,l}p_{ij}A_{jl}\overline{p_{kl}},
$$

so the new matrix is

$$
\boxed{P A\overline P^{\,T}}.
$$

The subspace $N=V^\perp$ is the [radical](../../../../../../radical-of-a-bilinear-form.md) of $H$. In coordinates it is the [kernel](../../../../../../kernel-of-a-linear-map.md) of $A$, and the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) gives

$$
\boxed{\dim N=n-\operatorname{rank}A}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

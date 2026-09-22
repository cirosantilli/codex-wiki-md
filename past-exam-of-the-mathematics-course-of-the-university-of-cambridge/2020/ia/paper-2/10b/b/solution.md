<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Writing $a_kx_k=\mathbf a\mathbin\cdot\mathbf x$ and differentiating gives

$$
d_{ij}=-\frac{a_ix_j}{r^3}
+\frac{a_jx_i}{r^3}
+\frac{(\mathbf a\cdot\mathbf x)\delta_{ij}}{r^3}
-\frac{3(\mathbf a\cdot\mathbf x)x_ix_j}{r^5}.
$$

Its [symmetric second-rank tensor](../../../../../../symmetric-second-rank-tensor.md) part and [antisymmetric second-rank tensor](../../../../../../antisymmetric-second-rank-tensor.md) part are

$$
d_{(ij)}=\frac{(\mathbf a\cdot\mathbf x)\delta_{ij}}{r^3}
-\frac{3(\mathbf a\cdot\mathbf x)x_ix_j}{r^5},
\qquad
d_{[ij]}=\frac{a_jx_i-a_ix_j}{r^3}.
$$

Taking the trace makes the two symmetric terms cancel, so the [divergence](../../../../../../divergence.md) is

$$
\boxed{\partial_i u_i=0}.
$$

Contracting the antisymmetric part with the Levi-Civita symbol gives the [curl](../../../../../../curl.md)

$$
\boxed{\nabla\times\mathbf u
=\frac{2\,\mathbf a\times\mathbf x}{r^3}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

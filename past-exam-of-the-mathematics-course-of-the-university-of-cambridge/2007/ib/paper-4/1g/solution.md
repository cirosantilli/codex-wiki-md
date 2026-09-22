<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [dual map](../../../../../transpose-of-a-linear-map.md) reverses the direction of the [linear map](../../../../../linear-map.md):

$$
\boxed{\alpha^*:W^*\longrightarrow V^*,\qquad \alpha^*(\lambda)=\lambda\circ\alpha.}
$$

Here the [dual spaces](../../../../../dual-space.md) consist of complex-linear [functionals](../../../../../functional.md). Composition with $\alpha$ is linear both as a [functional](../../../../../functional.md) on $V$ and as an operation on $W^*$, so this does define a [linear map](../../../../../linear-map.md) between the [dual spaces](../../../../../dual-space.md).

Let $(v_1,\ldots,v_n)$ and $(w_1,\ldots,w_m)$ be the chosen [bases](../../../../../basis.md), and let $(v^1,\ldots,v^n)$ and $(w^1,\ldots,w^m)$ be their [dual bases](../../../../../dual-basis.md). If $A$ represents $\alpha$, then $\alpha(v_i)=\sum_jA_{ji}w_j$. Therefore

$$
(\alpha^*w^j)(v_i)=w^j(\alpha(v_i))=A_{ji},\qquad\alpha^*w^j=\sum_iA_{ji}v^i.
$$

The coefficient in row $i$, column $j$ of the [matrix](../../../../../matrix.md) of $\alpha^*$ is thus $A_{ji}$, giving **the [matrix transpose](../../../../../transpose.md) $A^{\mathsf T}$**. This calculation introduces no [complex conjugation](../../../../../complex-conjugation.md): the algebraic [dual map](../../../../../transpose-of-a-linear-map.md) uses complex-linear [functionals](../../../../../functional.md), whereas a [Hermitian transpose](../../../../../conjugate-transpose.md) belongs to the inner-product adjoint construction.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

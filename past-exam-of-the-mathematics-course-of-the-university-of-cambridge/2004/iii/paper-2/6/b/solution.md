<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent a subset by the coordinate [vector](../../../../../../vector.md) of its [indicator function](../../../../../../indicator-function.md) in $\mathbb F_2^n$. [Symmetric difference](../../../../../../symmetric-difference.md) then becomes coordinatewise addition, and the proposed pairing is the [dot product](../../../../../../dot-product.md)

$$
B(x,y)=\sum_{i=1}^nx_iy_i.
$$

It is a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md), and it is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) because its [Gram matrix](../../../../../../gram-matrix.md) in the singleton basis is the identity. Coordinate [permutations](../../../../../../permutation.md) preserve the sum, so the natural $S_n$ action preserves the [bilinear form](../../../../../../bilinear-form.md).

Let $j=(1,\ldots,1)$, the [vector](../../../../../../vector.md) representing the full set. Then

$$
W=\langle j\rangle^\perp=\{x:\sum_ix_i=0\}
$$

is the even-weight subspace. For even $n$, $B(j,j)=n=0$ in $\mathbb F_2$, so $j\in W$. Moreover $B(x,x)=\sum_ix_i^2=\sum_ix_i=0$ for $x\in W$, making the restricted [bilinear form](../../../../../../bilinear-form.md) alternating. Nondegeneracy on the ambient space implies $W^\perp=\langle j\rangle$, so the radical of $B|_W$ is exactly

$$
W\cap W^\perp=\langle j\rangle.
$$

Thus it descends to an [alternating bilinear form](../../../../../../alternating-bilinear-form.md) on $W/\langle j\rangle$, independent of the representatives, and that quotient form has zero radical. **The induced form is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md)**, and its dimension is $n-2$. This is the [symplectic quotient of the binary subset module](../../../../../../symplectic-quotient-of-the-binary-subset-module.md); at $n=2$ it is the zero-dimensional [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) space.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

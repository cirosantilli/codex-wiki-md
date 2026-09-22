<h1 id="40c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An orthonormal eigenbasis is

$$
\mathbf v_9=\frac1{\sqrt3}(1,1,1)^T,
\qquad
\mathbf v_6=\frac1{\sqrt6}(1,-2,1)^T,
\qquad
\mathbf v_2=\frac1{\sqrt2}(1,0,-1)^T.
$$

The starting vector has the [orthogonal decomposition](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md)

$$
\mathbf x_0
=0\mathbf v_9+\frac{\sqrt3}{2}\mathbf v_6+\frac12\mathbf v_2.
$$

Hence its component in the dominant eigenspace is exactly zero. Normalizing $A^k\mathbf x_0$ gives

$$
\boxed{
\mathbf x_k
=
\frac{
6^k(1,-2,1)^T+2^k(1,0,-1)^T
}{
\sqrt2\sqrt{3\cdot36^k+4^k}
}
}.
$$

Since the two remaining eigenvectors are orthogonal,

$$
\boxed{
r(\mathbf x_k)
=\frac{18\cdot36^k+2\cdot4^k}
{3\cdot36^k+4^k}
}.
$$

Therefore

$$
\boxed{\lim_{k\to\infty}r(\mathbf x_k)=6}.
$$

The limit is not the leading eigenvalue $9$ because the nonorthogonality assumption in part (a) fails. On the [active spectrum of the power method](../../../../../../active-spectrum-of-the-power-method.md), the leading eigenvalue is $6$ and the next is $2$; indeed

$$
r(\mathbf x_k)-6
=-\frac{4\cdot4^k}{3\cdot36^k+4^k}
=O(3^{-2k}),
$$

in agreement with the squared spectral-ratio estimate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

The [first isomorphism theorem](../../../../../first-isomorphism-theorem.md) says that for a homomorphism $\phi:G\to H$,

$$
G/\ker\phi\cong\operatorname{im}\phi,
\qquad g\ker\phi\mapsto\phi(g).
$$

The map is well-defined because equal cosets differ by a kernel element; it is a surjective homomorphism onto the image, and injectivity follows because its kernel is the identity coset.

Here $GL_n(\mathbb R)$ consists of invertible real $n\times n$ [matrices](../../../../../matrix.md) and $SL_n(\mathbb R)$ consists of those with [determinant](../../../../../determinant.md) one. The latter is the kernel of the surjective [determinant](../../../../../determinant.md) map to $\mathbb R^*$, so it is normal and

$$
GL_n(\mathbb R)/SL_n(\mathbb R)\cong\mathbb R^*.
$$

The given [integral](../../../../../integral.md) [matrices](../../../../../matrix.md) form a [group](../../../../../group-split.md) because products and inverses remain [integral](../../../../../integral.md). The inverse formula shows that an [integral](../../../../../integral.md) inverse exists exactly when the [determinant](../../../../../determinant.md) divides every cofactor; taking [determinants](../../../../../determinant.md) shows more directly that $\det A\det A^{-1}=1$, hence $\det A=\pm1$, and the adjugate formula proves the converse. The [matrices](../../../../../matrix.md) $\left(\begin{smallmatrix}1&m\\0&1\end{smallmatrix}\right)$ show infinitude.

Reduction modulo two is a homomorphism $G\to GL_2(\mathbb F_2)$. Its kernel is exactly $H$, so $H$ is normal; its index is finite because the target has only six elements.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
